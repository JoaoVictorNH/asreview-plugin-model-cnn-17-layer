# ASReview CNN classifier
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5084887.svg)](https://doi.org/10.5281/zenodo.5084887)

This repository contains a plugin for [ASReview](https://github.com/asreview) ![logo](https://raw.githubusercontent.com/asreview/asreview-artwork/e2e6e5ea58a22077b116b9c3d2a15bc3fea585c7/SVGicons/IconELAS/ELASeyes24px24px.svg "ASReview"). This plugin adds a convolutional neural network (CNN) model, that has been shown to outperform classical algorithms in certain cases. It prefers [wide doc2vec](https://github.com/JTeijema/asreview-plugin-wide-doc2vec/) to work, but doc2vec works too.

## Getting started

The packaged is called `asreview-plugin-model-cnn-17-layer` and can be installed with:

```bash
pip install .
```
from the download folder or run the follow to install directly

```bash
pip install git+https://github.com/JoaoVictorNH/asreview-plugin-model-cnn-17-layer.git
```

## Usage
Note that the doc2vec feature extraction needs gensim installed.

The new convolutional neural network is implemented in [`asreviewcontrib/models/cnn.py`](asreviewcontrib/models/cnn.py) , usable with `-m power_cnn`:
```bash
asreview simulate benchmark:van_de_Schoot_2017 -m power_cnn -e doc2vec
```


## License
Apache-2.0 License 
