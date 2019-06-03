# Setup for cluster envorinment of conda


## Install Tensorflow
```bash
conda install tensorflow-gpu keras opencv ipyparallel dask-glm dask-ml dask-searchcv nodejs cvxopt 
```

## Install others
```bash
conda install -c cvxgrp cvxpy
```

# NoMachine Error
if nomachine starts acting really weird (like terminal is not responding, or your keyboard input doesn't work right) you can usually fix it by: 
1) killing the current nomachine process (use a regular terminal to ssh into whichever login node you are using, use `kill $PID` where `$PID` corresponds to the PID for `nxnode.bin` )
2) move/rename your `.bash_profile` file
3) start up a nomachine session again (it should work now)
4) don't forget to un-rename your `.bash_profile` file
