# kdtree comparison

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This was a side project of developing [py4dgeo](https://github.com/ssciwr/py4dgeo).
In a Jupyter notebook, the performance of the following KDTree implementations was studies:

* PCL (using the FLANN library)
* NanoFLANN
* SciPy
* scikit-learn

This repository conserves this experiment. The main comparison is `jupyter/searchtree.ipynb`.
The final decision was to use NanoFLANN for `py4dgeo`.

## Reproducing

The experiments can be reproduced with a Docker container.
The image can be locally built and run with the following commands:

```
docker build -t kdtree-comparison:latest .
docker run -t -p 8888:8888 kdtree-comparison:latest
```
