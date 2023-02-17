# PyTorch-research
Repo for PyTorch research and development, specifically using ROCm GPU acceleration, the Apple Metal Framework, and the Intel PyTorch for GPU extension.

# Getting started
## Install PyTorch - Radeon
Install PyTorch for ROCm 5.2 for Linux with Pip -- [pytorch](https://pytorch.org/get-started/locally/)<br>

`pip3 install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/rocm5.2`

This assumes you are using one of the following linux distributions:
- Arch Linux, *minimum version 2012-07-15*
- CentOS, *minimum version 7.3-1611*
- Debian, *minimum version 8.0*
- Fedora, *minimum version 24*
- Mint, *minimum version 14*
- OpenSUSE, *minimum version 42.1*
- PCLinuxOS, *minimum version 2014.7*
- Slackware, *minimum version 14.2*
- Ubuntu, *minimum version 13.04*

And a ROCm 5.2 supported GPU:
- Radeon Instinct MI100, MI50, MI125
- AMD Radeon VII
- AMD Radeon RX 5700, RX 5700 XT
- AMD Radeon RX 6800, RX 6800 XT, RX 6900 XT
- AMD Radeon Pro VII, WX 9100, WX 8200, WX 7100
- AMD Radeon Instinct MI60, MI50x, MI25x, MI8
- AMD Radeon RX Vega 64, RX Vega 56, RX 580, RX 480<br>

*Note: not all features may be supported on all GPUs, and some features may require specific hardware configurations or BIOS settings. Also, keep in mind that newer versions of ROCm may support additional GPUs or features, so it's always a good idea to check the ROCm documentation for the latest information.*

## Install PyTorch - Metal
Install PyTorch for Mac with the default compute platform with Pip -- [pytorch](https://pytorch.org/get-started/locally/)

`pip3 install torch torchvision torchaudio`

## Install ROCm 5.2 - Ubuntu
Add ROCm repository to your system.<br>
`wget -q0 - https://repo.radeon.com/rocm/rocm.gpg.key | sudo apt-key add -`<br>
`echo 'deb [arch=amd64] https://repo.radeon.com/rocm/apt/5.2/ ubuntu main' | sudo tee /etc/apt/sources.list.d/rocm.list`

