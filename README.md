# EarthAnnotator

> Rapid image labeling for data-driven Earth science discovery.

A tool for web-based image annotation and efficient labeling pixels in images 

Implements a rapid technique, described by [Buscombe & Ritchie, (2018)](https://www.mdpi.com/2076-3263/8/7/244), for dense image labeling based on limited manual annotations.

Credits: Thanks to code contributions from [Colin Talbert](https://github.com/talbertc-usgs) and [Rich Signell](https://github.com/rsignell-usgs)  

## Run online through your browser:

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/dbuscombe-usgs/EarthAnnotator/master?filepath=EarthAnnotator.ipynb)

Example instructional video [here](https://www.youtube.com/watch?v=oGKWWCb_Bvs&feature=youtu.be)


## Install on your own computer

First, if you're a regular conda user, you should start by doing some housekeeping:

```
conda clean --all
conda update anaconda
conda update conda
conda update --all
```

Clone the repository:

```
git clone https://github.com/dbuscombe-usgs/EarthAnnotator.git
```

```
conda config --remove channels conda-forge
```


Create a conda environment:

```
conda config --add channels conda-forge
conda env create -f binder\environment.yml
```

Activate the conda environment (called ```EA```):

```
conda activate EA
```

```
conda config --remove channels conda-forge
```


Add the kernel to jupyter:

```
python -m ipykernel install --user --name EA --display-name "Python (earthannotator)"
```

Have a look at the kernels 

```
jupyter kernelspec list
```


Run the notebook (shows up in your web browser):

```
jupyter notebook
```




