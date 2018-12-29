# install-Tensorflow-on-Drive-PX2

Install tensorflow on NVIDIA DRIVE PX2(AutoChauffeur)

# Setup Environment
export PATH=/usr/local/cuda/bin:$PATH\n
export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH\n
export LD_LIBRARY_PATH=/usr/local/cuda/extras/CUPTI/lib64:$LD_LIBRARY_PATH\n

# Install pip
- for python 2.7\n
sudo apt-get install python-pip\n

- for python 3.6
sudo apt-get install python-pip

# Install tensorflow 1.9
- for python 2.7
pip install --extra-index-url=https://developer.download.nvidia.com/compute/redist/jp33 tensorflow-gpu

- for python 3.6
pip3 install --extra-index-url=https://developer.download.nvidia.com/compute/redist/jp33 tensorflow-gpu
