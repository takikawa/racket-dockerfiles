# Dockerfile for Racket's pre-release build
#
# Version 0.1

FROM ubuntu

MAINTAINER Asumu Takikawa, asumu@racket-lang.org

# Get required packages to fetch and run Racket
RUN apt-get update
RUN apt-get install -y wget git libcairo2 libpango1.0-0 libjpeg8

# Download the current snapshot and install it
RUN wget http://www.cs.utah.edu/plt/snapshots/current/installers/racket-current-x86_64-linux-precise.sh
RUN sh racket-current-x86_64-linux-precise.sh --unix-style
