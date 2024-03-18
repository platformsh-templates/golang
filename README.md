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

## Configuration

This repository contains configuration files within the `.platform` and `.upsun` directories for deploying to Platform.sh and Upsun, respectively.
If you deploy on Platform.sh, feel free to remove the Upsun config files (and vice versa).
