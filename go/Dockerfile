FROM golang:latest

ARG PUID=1000
ARG PGID=1000

ENV PUID ${PUID}
ENV PGID ${PGID}

RUN groupadd -g ${PGID} gueroverde && \
    useradd -u ${PUID} -g gueroverde -m gueroverde && \
    apt-get update -yqq

WORKDIR /var/go

ENV GOROOT /usr/local/go
ENV GOPATH /var/go
RUN mkdir /var/go/pkg
RUN mkdir /var/go/src
RUN mkdir /var/go/bin
ENV GOBIN ${GOPATH}/bin
ENV PATH ${PATH}:/usr/local/bin:${GOROOT}/bin:${GOBIN}

# Set default work directory

RUN chown -R gueroverde:gueroverde /var/go

WORKDIR /var/go

