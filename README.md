Dockerfiles for Racket
----------------------

[Docker.io](https://www.docker.io/) allows the creation of lightweight software containers
using LXC and cgroups. The Dockerfiles in this repository can be used to build Docker
containers that include an installation of the [Racket](http://racket-lang.org) programming
language.

Docker containers with Racket may be useful for deploying Racket-based web applications.

How to use
----------

If you already have Docker installed, take the following steps to build an image:

  * `git clone https://github.com/takikawa/racket-dockerfiles.git`
  * `cd racket-dockerfiles/<dir>`
  * `docker build .`

where `<dir>` is one of the Dockerfile directories. For example, the
`head` directory contains a Dockerfile that builds the latest Racket from
the git repository.

Once the image is built, you can run it:

  `docker run -i <image-id>`

which will bring up a Racket REPL. To find out what `<image-id>` is, inspect the
output of `docker images`.

On Debian, the `docker` executable is called `docker.io`.

---

Copyright © 2014 Asumu Takikawa

This software is distributed under the MIT License. See the LICENSE file.
