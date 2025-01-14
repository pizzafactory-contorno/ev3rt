FROM pizzafactory0contorno/piatto:debian-11@sha256:d6841bd91f71d65dade870204c47f66ee767c96e2ba9f5857ebec64721316446

RUN sudo apt-get update \
 && sudo apt-get upgrade -y \
 && sudo apt-get install -y wget bzip2 build-essential ruby \
 && wget http://ev3rt-git.github.io/public/ev3rt-prepare-ubuntu.sh \
 && yes 1 | sudo bash -x ev3rt-prepare-ubuntu.sh \
 && sudo rm ev3rt-prepare-ubuntu.sh \
 && sudo apt-get clean \
 && sudo rm -rf /var/lib/apt/lists/*
