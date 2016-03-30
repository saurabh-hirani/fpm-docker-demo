FROM shirani/precise-tool
MAINTAINER Saurabh Hirani <saurabhhirani@bluejeansnet.com>
ENV DEBIAN_FRONTEND=noninteractive

COPY . /build

RUN cd /build && bin/create-fpm-pkg server /artifacts

VOLUME /artifacts
