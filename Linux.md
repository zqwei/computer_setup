# Setup for cluster envorinment of conda

## Old version of anaconda (python 3.5)
https://repo.continuum.io/archive/Anaconda3-4.2.0-MacOSX-x86_64.pkg

## Install Tensorflow
```bash
conda install -c anaconda tensorflow 
```
## Install Keras
```bash
conda install -c anaconda keras
```
## Install OpenCV
```bash
conda install -c anaconda opencv
```
## Install others
```bash
conda install -c conda-forge tqdm
conda install -c anaconda ipyparallel future
conda install -c cvxgrp cvxpy libgcc
conda install -c anaconda cvxopt
```

## Install Node.JS
```bash
conda install -c conda-forge nodejs
```

## Install TexLive
```bash
conda install -c conda-forge texlive-core
```

## Install Dask
```bash
conda install -c conda-forge dask-ml
conda install -c conda-forge dask-drmaa
```

## Install Imaging packages
```bash
pip install -e CaImAn
cd trefide/src
make clean
make
LDSHARED="icc -shared" CC=icc CXX=icpc pip install -e trefide
pip install -e funimag
```

# NoMachine Error
if nomachine starts acting really weird (like terminal is not responding, or your keyboard input doesn't work right) you can usually fix it by: 
1) killing the current nomachine process (use a regular terminal to ssh into whichever login node you are using, use `kill $PID` where `$PID` corresponds to the PID for `nxnode.bin` )
2) move/rename your `.bash_profile` file
3) start up a nomachine session again (it should work now)
4) don't forget to un-rename your `.bash_profile` file
