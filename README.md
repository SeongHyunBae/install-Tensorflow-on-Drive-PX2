# install-Tensorflow-on-Drive-PX2

Install tensorflow on NVIDIA DRIVE PX2(AutoChauffeur)  
CUDA Version 9.0, CUDNN Version 7  
(check cuda version by writing 'cat /usr/local/cuda/version.txt' in terminal)  
(check cudnn version by writing 'cat /usr/include/cudnn.h | grep CUDNN_MAJOR -A 2' in terminal)  

# Setup Environment
export PATH=/usr/local/cuda/bin:$PATH  
export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH  
export LD_LIBRARY_PATH=/usr/local/cuda/extras/CUPTI/lib64:$LD_LIBRARY_PATH  

# Install pip
- for python 2.7  
sudo apt-get install python-pip  

- for python 3.6  
sudo apt-get install python3-pip  

# Install tensorflow 1.9.0
- for python 2.7  
pip install --extra-index-url=https://developer.download.nvidia.com/compute/redist/jp33 tensorflow-gpu  

- for python 3.6  
pip3 install --extra-index-url=https://developer.download.nvidia.com/compute/redist/jp33 tensorflow-gpu  

# Install tensorflow 1.11.0
- for python 2.7
sudo apt-get install libhdf5-serial-dev hdf5-tools  
pip install h5py  
And download file in here: https://nvidia.app.box.com/v/JP33-TF1-11-0-py27-wTRT  
cd Downloads  
pip install tensorflow-1.11.0-cp27-cp27mu-linux_aarch64.whl  

- for python 3.6  
sudo apt-get install libhdf5-serial-dev hdf5-tools  
pip3 install h5py  
And download file in here: https://nvidia.app.box.com/v/JP33-TF1-11-0-py35-wTRT  
cd Downloads  
pip3 install tensorflow-1.11.0-cp35-cp35m-linux_aarch64.whl
