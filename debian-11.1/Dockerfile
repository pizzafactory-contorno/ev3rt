FROM pizzafactory0contorno/piatto:debian-11@sha256:fe2d63a9461c67205151fac96ece7b3dde4f6d40a3c29114c86409454c812562

RUN sudo apt-get update \
 && sudo apt-get upgrade -y \
 && sudo apt-get install -y wget bzip2 build-essential ruby \
 && wget http://ev3rt-git.github.io/public/ev3rt-prepare-ubuntu.sh \
 && yes 1 | sudo bash -x ev3rt-prepare-ubuntu.sh \
 && sudo rm ev3rt-prepare-ubuntu.sh \
 && sudo apt-get clean \
 && sudo rm -rf /var/lib/apt/lists/*
