# Setup for cluster envorinment of conda

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
