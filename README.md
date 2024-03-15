> [!IMPORTANT]
> **Archived code example**
>
> Public code examples for Platform.sh, Upsun, and Blackfire.io are proof of concepts.
> Feel free to use them as a starting reference for your work, but know that they are generally unmaintained once published.

![golang](https://socialify.git.ci/platformsh/golang/image?description=1&descriptionEditable=%E2%9A%97%EF%B8%8F%20Deploy%20often.%20%F0%9F%9A%80%20Deploy%20Friday!&font=Jost&language=1&logo=https%3A%2F%2Fplatform.sh%2Fplatform-logos%2Ficons%2Fwhite%2FPlatformsh_Icon_white.svg&name=1&owner=1&pattern=Solid&theme=Dark)

This template provides the most basic configuration for running a custom Go project using Go modules.  It demonstrates the Platform.sh `config-reader` library and connecting to a MariaDB instance.  It can be used to build a very rudimentary application but is intended primarily as a documentation reference.

Go is a statically typed, compiled language with an emphasis on easy concurrency and network services.

<p align="center">
    <br/>
<a href="https://console.platform.sh/projects/create-project?template=https://github.com/platformsh/golang.git&utm_content=golang&utm_source=github&utm_medium=button&utm_campaign=deploy_on_platform">
    <img src="https://platform.sh/images/deploy/lg-blue.svg" alt="Deploy on Platform.sh" width="200px" />
</a>
</p>

## Features

* Go 1.16
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
