# CUDA 10 Installation Guide on Ubuntu 18.04

## Install GPU Driver:
```
sudo add-apt-repository ppa:graphics-drivers/ppa
sudo apt install nvidia-driver-410
reboot
```
After reboot check if the driver is installed properly by:
```
nvidia-smi
```

## Install CUDA 10 using runfile:
```
chmod +x ./cuda_10.0.130_410.48_linux.run
./cuda_10.0.130_410.48_linux.run --extract=$HOME
~/.cuda-linux.10.0.130-24817639.run
echo 'export CUDA_HOME=/usr/local/cuda' > ~/.bashrc
echo 'export PATH=/usr/local/cuda/bin:$PATH'
reboot
```
After reboot check if CUDA 10 is installed properly by:
```
nvcc --version
```
## Install CuDNN:
```
sudo dpkg -i libcudnn7_7.4.1.5-1+cuda10.0_amd64.deb
sudo dpkg -i libcudnn7-dev_7.4.1.5-1+cuda10.0_amd64.deb
```
