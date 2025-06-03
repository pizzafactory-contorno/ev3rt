FROM pizzafactory0contorno/piatto:debian-11@sha256:6bb27f0f90155655a5b832bc78b5e0a7eb3bad4bfed7a3f9fa4ab081beac22c1

RUN sudo apt-get update \
 && sudo apt-get upgrade -y \
 && sudo apt-get install -y wget bzip2 build-essential ruby \
 && wget http://ev3rt-git.github.io/public/ev3rt-prepare-ubuntu.sh \
 && yes 1 | sudo bash -x ev3rt-prepare-ubuntu.sh \
 && sudo rm ev3rt-prepare-ubuntu.sh \
 && sudo apt-get clean \
 && sudo rm -rf /var/lib/apt/lists/*
