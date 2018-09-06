## Python

### GPU Accelerated Math Libraries: pyculib
Pyculib is a package that provides access to several numerical libraries that are optimized for performance on NVidia GPUs. Pyculib was originally part of Accelerate, developed by Anaconda, Inc.

```bash
conda update conda
conda install pyculib
```

### Deep Learning: Keras, TensorFlow, PyTorch
Keras and the GPU-enabled version of TensorFlow can be installed in Anaconda with the command
```bash
conda install keras-gpu
```

### GPU Kernel Programming: Numba
Numba’s GPU support is optional, so to enable it you need to install both the Numba and CUDA toolkit conda packages:
```bash
conda install numba cudatoolkit
```

### GPU Dataframes: PyGDF

### Cupy
```bash
conda install -c anaconda cupy 
```

### Pytorch SRU units
https://github.com/taolei87/sru
