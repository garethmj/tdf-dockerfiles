FROM ubuntu:16.04

RUN \
  apt-get update && \
  apt-get -y upgrade && \
  apt-get install -y curl git vim && \
  rm -rf /var/lib/apt/lists/*

ENV HOME /root

WORKDIR /root

CMD ["bash"]