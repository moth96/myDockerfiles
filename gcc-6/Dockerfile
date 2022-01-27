FROM gcc:6.3.0
RUN groupadd yhz && useradd -ms /bin/bash -d /home/yhz -g yhz yhz
USER yhz:yhz
RUN mkdir -p /home/yhz/build
COPY --chown=yhz:yhz . /home/yhz/build
WORKDIR /home/yhz/build