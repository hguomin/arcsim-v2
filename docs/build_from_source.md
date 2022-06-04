# Instructions for building the source code.

## Development environment
- Ubuntu 20.04  
- Python 3

## Install dependent packages
```bash
sudo apt-get install gcc make g++ libboost-all-dev freeglut3-dev \
          gfortran liblapacke-dev libpng-dev libpng++-dev scons \
          libatlas-base-dev ctags libopenblas-dev
```

when building the `jsoncpp` in the `dependencies` folder, the build tool scons will use the system default python3 to build, so need to install the `apply` package to system default python3 using below command.
```bash
pip3 install apply
```
## Build the code
```bash
git clone https://github.com/hguomin/arcsim-v2.git
cd arcsim-v2/dependencies
make

cd ..
make

```

## References  
https://github.com/DanielTakeshi/ARCSim-Installation-Instructions  