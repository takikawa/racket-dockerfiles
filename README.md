Dockerfiles for Racket
----------------------

[Docker.io](https://www.docker.io/) allows the creation of lightweight software containers
using LXC and cgroups. The Dockerfiles in this repository can be used to build Docker
containers that include an installation of the [Racket](http://racket-lang.org) programming
language.

Docker containers with Racket may be useful for deploying Racket-based web applications.

How to use
----------

If you already have Docker installed, take the following steps:

  * `git clone https://github.com/takikawa/racket-dockerfiles.git`
  * `cd racket-dockerfiles/<dir>`
  * `docker build .`

where `<dir>` is one of the Dockerfile directories. For example, the
`head` directory contains a Dockerfile that builds the latest Racket from
the git repository.

On Debian, the `docker` executable is called `docker.io`.
