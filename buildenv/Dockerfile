FROM randomdude/gcc-cross-x86_64-elf

RUN echo "deb http://archive.debian.org/debian/ stretch main" > /etc/apt/sources.list
RUN echo "Acquire::Check-Valid-Until false;" > /etc/apt/apt.conf.d/99no-check-valid-until
RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install -y nasm
RUN apt-get install -y xorriso
RUN apt-get install -y grub-pc-bin
RUN apt-get install -y grub-common

VOLUME /root/env
WORKDIR /root/env
