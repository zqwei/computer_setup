# Setup for cluster envorinment of conda

## Old version of anaconda (python 3.5)
https://repo.continuum.io/archive/Anaconda3-4.2.0-MacOSX-x86_64.pkg

## Install Tensorflow
```bash
conda install -c conda-forge tensorflow keras opencv tqdm ipyparallel future cvxopt nodejs dask-ml dask-drmaa
```

## Install others
```bash
conda install -c cvxgrp cvxpy libgcc
```

## Install TexLive
```bash
conda install -c conda-forge texlive-core
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
