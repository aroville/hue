# Welcome to Hue (http://gethue.com) Dockerfile
# Build an image from a remote github or local cloned Hue repository.

FROM ubuntu:18.04
LABEL description="Hue Project https://github.com/cloudera/hue"

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update -y && apt-get install -y \
    build-essential \
    libkrb5-dev \
    libmysqlclient-dev \
    libssl-dev \
    libsasl2-dev \
    libsasl2-modules-gssapi-mit \
    libsqlite3-dev \
    libtidy-dev \
    libxml2-dev \
    libxslt-dev \
    libffi-dev \
    libldap2-dev \
    libpq-dev \
    asciidoc \
    python-dev \
    python-setuptools \
    libgmp3-dev \
    libz-dev \
    software-properties-common \
    curl \
    git \
    rsync \
    sudo \
    maven \
    gcc \
    swig \
    # openssl \ # Breaks build
    xmlsec1 \
    libxmlsec1-openssl \
    hugo \
    && rm -rf /var/lib/apt/lists/*

# Need recent version for Ubuntu
RUN curl -sL https://deb.nodesource.com/setup_10.x | sudo bash - \
    && apt-get install -y nodejs

ENV HOME=/tmp

