FROM pizzafactory0contorno/piatto:debian-11@sha256:6653d54081c7609d20389a7e169c333ae347707ce4f67736feb5bc1da59f2e46

RUN sudo apt-get update \
 && sudo apt-get upgrade -y \
 && sudo apt-get install -y wget bzip2 build-essential ruby \
 && wget http://ev3rt-git.github.io/public/ev3rt-prepare-ubuntu.sh \
 && yes 1 | sudo bash -x ev3rt-prepare-ubuntu.sh \
 && sudo rm ev3rt-prepare-ubuntu.sh \
 && sudo apt-get clean \
 && sudo rm -rf /var/lib/apt/lists/*
