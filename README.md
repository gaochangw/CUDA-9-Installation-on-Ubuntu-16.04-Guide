# CUDA-9-Installation-on-Ubuntu-16.04-Guide
CUDA 9 Installation on Ubuntu 16.04 Guide

## Install Third-party Libraries:
sudo apt-get install g++ freeglut3-dev build-essential libx11-dev libxmu-dev libxi-dev libglu1-mesa libglu1-mesa-dev

## Quit X Server
CTRL + ALT + F1
sudo service lightdm stop
sudo init 3

## Install CUDA 9 using runfile:
chmod +x ./your-nvidia-file.run
sudo ./cuda


