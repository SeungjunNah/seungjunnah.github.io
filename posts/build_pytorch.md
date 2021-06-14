# [Publications](publications) | [Datasets](Datasets/datasets) | [CV](cv.pdf)
___

# Install pytorch from source

Tested with Ubuntu 20.04

## Install GPU libraries

* cuda & nvidia driver

```bash
wget https://developer.download.nvidia.com/compute/cuda/11.3.1/local_installers/cuda_11.3.1_465.19.01_linux.run

# Check your OS version!
# install the latest driver & cudatoolkit
# NEVER!! create a symbolic link at /usr/local
sudo sh cuda_11.3.1_465.19.01_linux.run
```

* cudnn

Visit [cudnn download page](https://developer.nvidia.com/rdp/cudnn-download)

Choose `Download cuDNN v8.2.0 (April 23rd, 2021), for CUDA 11.x`
`cuDNN Library for Linux (x86_64)`
```bash
tar -xf cudnn-11.3-linux-x64-v8.2.0.53.tgz
cd cuda/
sudo cp -rf include/* /usr/local/cuda-11.3/include/
sudo cp -rf lib64/* /usr/local/cuda-11.3/lib64/
```

* nccl

Visit [NCCL download page](https://developer.nvidia.com/nccl/nccl-download)
Choose `Download NCCL 2.9.8, for CUDA 11.3, May 11, 2021`
`O/S agnostic local installer`

```bash
tar -xf nccl_2.9.8-1+cuda11.3_x86_64.txz
sudo cp -rf nccl_2.9.8-1+cuda11.3_x86_64 /usr/local/
```

* set environment variables

Open your `~/.bashrc`

```bash
CUDA_HOME=/usr/local/cuda-11.3

if [ -z $LD_LIBRARY_PATH ]; then
  LD_LIBRARY_PATH=$CUDA_HOME/lib64
else
  LD_LIBRARY_PATH=$CUDA_HOME/lib64:$LD_LIBRARY_PATH
fi

export PATH=$CUDA_HOME/bin:$PATH

# nccl
export NCCL_HOME=/usr/local/nccl_2.9.8-1+cuda11.3_x86_64
export NCCL_LIB_DIR=$NCCL_HOME/lib
export PATH=$NCCL_HOME/include:$NCCL_HOME/lib:$PATH
export LD_LIBRARY_PATH=$NCCL_HOME/lib:$LD_LIBRARY_PATH
```

## Set conda environment

```bash
conda create -n pytorch_s python=3.8 imageio tqdm requests scikit-image -y
conda activate pytorch_s

conda install astunparse numpy ninja pyyaml mkl mkl-include setuptools cmake cffi typing_extensions future six requests dataclasses -y

conda install -c pytorch magma-cuda113 -y

```


## Build from source

* pytorch

```bash
mkdir ~/local
cd ~/local

git clone --recursive https://github.com/pytorch/pytorch
cd pytorch

git submodule sync
git submodule update --init --recursive

export CMAKE_PREFIX_PATH=${CONDA_PREFIX:-"$(dirname $(which conda))/../"}
BUILD_CAFFE2=0 USE_SYSTEM_NCCL=1 python setup.py install
# as long as you don't need caffe2, this reduces the building time.
# due to NCCL detection bug in pytorch. It might be fixed later.
```

* torchvision

```bash
git clone https://github.com/pytorch/vision
cd vision

python setup.py install
```