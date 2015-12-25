FROM ubuntu:16.04

RUN \
  apt-get update && \
  apt-get -y upgrade && \
  apt-get install -y \
  	ca-certificates \
  	curl \
  	git \
  	vim && \
  apt-get clean autoclean && apt-get autoremove -y && \
  rm -rf /var/lib/{apt,dpkg,cache,log}/

ENV HOME /root

WORKDIR /root

CMD ["bash"]