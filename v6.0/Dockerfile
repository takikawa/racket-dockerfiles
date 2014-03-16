# Dockerfile for building Racket v6.0
#
# Version 0.1

FROM ubuntu

MAINTAINER Asumu Takikawa, asumu@racket-lang.org

# Get required packages to build and use Racket
RUN apt-get update
RUN apt-get install -y wget make gcc libcairo2 libpango1.0-0 libjpeg8

# Download the src tarball and build Racket
RUN wget http://mirror.racket-lang.org/installers/6.0/racket-6.0-src-builtpkgs-unix.tgz
RUN tar -xvzf racket-6.0-src-builtpkgs-unix.tgz
RUN mkdir racket-6.0/src/build
RUN cd racket-6.0/src/build && ../configure --prefix=/usr && make && make install

ENTRYPOINT ["/usr/bin/racket"]
