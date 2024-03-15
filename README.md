> [!WARNING]
> **Unmaintained code example**
>
> Public code examples are proof of concepts.
> Feel free to use them as a starting reference for your work, but remember that they are generally unmaintained once published.

# Basic Go for Platform.sh

This template provides the most basic configuration for running a custom Go project using Go modules.  It demonstrates the Platform.sh `config-reader` library and connecting to a MariaDB instance.  It can be used to build a very rudimentary application but is intended primarily as a documentation reference.

Go is a statically typed, compiled language with an emphasis on easy concurrency and network services.

## Features

* Go 1.14
* MariaDB 10.4
* Automatic TLS certificates
* Git module-based build

## Customizations

This project relies on Go module support in Go 1.11 and later.  You should commit your `go.mod` and `go.sum` files to Git, but not the `vendor` directory.

The following files and additions make the framework work.  If using this project as a reference for your own existing project, replicate the changes below to your project.

* The `.platform.app.yaml`, `.platform/services.yaml`, and `.platform/routes.yaml` files have been added.  These provide Platform.sh-specific configuration and are present in all projects on Platform.sh.  You may customize them as you see fit.
* An additional Go module, [`platformsh/config-reader-go`](https://github.com/platformsh/config-reader-go), has been added.  It provides convenience wrappers for accessing the Platform.sh environment variables.

## References

* [Go](https://golang.org/)
* [Go on Platform.sh](https://docs.platform.sh/languages/go.html)
