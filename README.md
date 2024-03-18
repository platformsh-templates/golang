> [!IMPORTANT]
> **Archived code example**
>
> Public code examples for Platform.sh, Upsun, and Blackfire.io are proof of concepts.
> Feel free to use them as a starting reference for your work, but know that they are generally unmaintained once published.

# Go

This template provides the most basic configuration for running a custom Go project using Go modules.  It demonstrates the Platform.sh `config-reader` library and connecting to a MariaDB instance.  It can be used to build a very rudimentary application but is intended primarily as a documentation reference.

Go is a statically typed, compiled language with an emphasis on easy concurrency and network services.

<p align="center">
    <br/>
    <img src="https://platform.sh/images/deploy/lg-blue.svg" alt="Deploy on Platform.sh" width="180px" />
</a>
</p>

## Features

* Go 1.22
* MariaDB 11.2
* Automatic TLS certificates
* Git module-based build

## Customizations

This project relies on Go module support in Go 1.11 and later.  You should commit your `go.mod` and `go.sum` files to Git, but not the `vendor` directory.

The following files and additions make the framework work.  If using this project as a reference for your own existing project, replicate the changes below to your project.
