FROM ubuntu:jammy
LABEL maintainer="theenawman"
LABEL description="Dockerfile for base image with tools installed"

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && \
    apt-get install -qqy --no-install-recommends wget sudo nano && \
    apt-get -qy clean \
    autoremove \
    && rm -rf /var/lib/apt/lists/*

CMD ["/bin/bash"]
