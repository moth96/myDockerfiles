FROM ubuntu:32
RUN apt-get update && apt-get install -y nasm
RUN groupadd yhz && useradd -ms /bin/bash -d /home/yhz -g yhz yhz
USER yhz:yhz
RUN mkdir -p /home/yhz/build
COPY --chown=yhz:yhz . /home/yhz/build
WORKDIR /home/yhz/build