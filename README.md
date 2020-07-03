
# cytograph

## What's this?

This repo contains a collection of algorithms used in our paper "Molecular architecture of the mouse nervous system", currently in review. We provide it here in the interest of transparency and reproducibility. However, we are unable to provide support or documentation for using the code at this time. The instructions below can serve as a starting point.

Please check out instead the new repo [cytograph2](https://github.com/linnarsson-lab/cytograph2).

## Installation

The following instructions should work for Linux and Mac (unfortunately, we have no 
experience with Windows).

1. [Install Anaconda](https://www.continuum.io/downloads), Python 3.6 version

2. Install `loompy`:

```
git clone https://github.com/linnarsson-lab/Loom.git
cd Loom/python
python setup.py install
```

3. Install `cytograph`:

```
git clone https://github.com/linnarsson-lab/cytograph.git
cd cytograph/bhtsne
g++ sptree.cpp tsne.cpp -o bh_tsne -O2
cd ..
python setup.py install
```

Make sure `bhtsne` is in your $PATH

## Running the pipeline

**Note:** pipelines are now separated out into their own repos:

* [Adolescent mouse brain](https://github.com/linnarsson-lab/adolescent-mouse)

