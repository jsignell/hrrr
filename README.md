# Intro to Python Data Analysis - Xarray - Dask

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jsignell/hrrr/main?urlpath=lab)

Materials for **Intro to Python Data Analysis - Xarray - Dask** delivered in the **Open Science in Action** tutorials at the AGU Fall Meeting 2021.

## Summary
This is a tutorial about using Xarray and Dask to work with distributed computation on arrays in Python. We will learn how n-dimensional arrays are represented and can be manipulated using Python.If you often run out of memory or spend a long time running computations, this tutorial might help.

## Learner profile
This material is best suited to people who are familiar with Python (or another programming language like R, Matlab, or Julia). If you have encountered Pandas and Numpy and are familiar with running code in a Jupyter notebook even better!

## Learning Objectives
 After attending this, you should be able to:

- Load NetCDF, zarr, and geotiff data from local and remote storage.
- Subset your data to an region of interest without pulling the whole dataset into memory.
- Apply some linear algebra operations to labeled n-dimensional arrays without using for-loops.
- Understand what attributes and coordinates mean for Xarray objects.
- Set up lazy computation that run across a distributed set of machines using Dask.

## Local setup

To set up a local environment, first clone this repo and the data repo, then create the conda environment:

```
git clone https://github.com/jsignell/hrrr.git
cd hrrr
git clone https://github.com/pangeo-data/tutorial-data.git
conda env create -f binder/environment.yml  # or mamba env create...
conda activate hrrr
```

## Prior materials

This material is largely based off of the [Pangeo Xarray tutorial](http://gallery.pangeo.io/repos/pangeo-data/pangeo-tutorial-gallery/xarray.html) with the HRRR example inspired by [Rich Signell's](https://github.com/rsignell) [HRRR Best Time Series notebook](https://nbviewer.org/gist/rsignell-usgs/9d24820bcf6bf30a410eed1e891f3562). 

The GitHub repo is based off of [James Bourbeau's](https://github.com/jrbourbeau) [Dask binder template](https://github.com/jrbourbeau/dask-binder-template).
