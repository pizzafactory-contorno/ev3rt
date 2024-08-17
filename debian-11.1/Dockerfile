FROM pizzafactory0contorno/piatto:debian-11@sha256:9c04112ec1e4e76818d9245271d69fadddb08b1a1345e6b62c23797d4d71c9ff

RUN sudo apt-get update \
 && sudo apt-get upgrade -y \
 && sudo apt-get install -y wget bzip2 build-essential ruby \
 && wget http://ev3rt-git.github.io/public/ev3rt-prepare-ubuntu.sh \
 && yes 1 | sudo bash -x ev3rt-prepare-ubuntu.sh \
 && sudo rm ev3rt-prepare-ubuntu.sh \
 && sudo apt-get clean \
 && sudo rm -rf /var/lib/apt/lists/*
