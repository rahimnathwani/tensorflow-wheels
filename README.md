Recent official Tensorflow releases for x86 are built to use instruction sets not found on older CPUs (e.g. AVX). My desktop computer has enough power (Xeon X5675, GTX 1080) and RAM (48GB) for my needs, so I don't feel the need to upgrade just yet.

I re-compiled Tensorflow using the instructions: https://www.tensorflow.org/install/source

I used the latest-devel-gpu-py3 docker container, but made a few adjustments (switched branches from r1.12 to r1.13, installed python 3.7, upgraded some Nvidia libraries).

The built wheel works for my environment and can be installed with pip:

- Xeon X5675
- GTX 1080 (CUDA compute capability 6.1)
- python 3.7
- CUDA Toolkit 10.0
- CUDNN 7
