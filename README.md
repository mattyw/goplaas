See doc.go.

This is a fork of the goplay code included in misc/goplay of the go1.2 release.

The goal was to make a go playground that would allow you to make runnable examples using your ownpackages

It's a proof of concept to show how you can include runnable examples for your own
packages on your own webserver

To run the default server but point to a different server for doing the compilation do:

```bash
go run goplay.go -compile <url>
```

The real intention is that the server allows compile to be called from any origin.

This means the server can be run on a server with access to any packages in the GOPATH.

You can then include runnable examples on your website that point to this server for doing the compilation

