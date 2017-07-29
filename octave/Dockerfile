FROM ubuntu:latest
MAINTAINER Ruslan Sakevych

RUN apt-get update \
 && apt-get install -y software-properties-common less \
 && apt-add-repository ppa:octave/stable \
 && apt-get update \
 && apt-get install -y octave \
 && rm -rf /var/lib/apt/lists/*

WORKDIR "/source"

CMD ["octave", "--no-gui"]
