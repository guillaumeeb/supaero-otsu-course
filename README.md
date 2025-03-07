# Course and exercice on Satellite imagery analysis using Xarray and Dask

[![Binder](http://mybinder.org/badge_logo.svg)](http://mybinder.org/v2/gh/guillaumeeb/supaero-otsu-course/HEAD?urlpath=lab/tree/ndsi.ipynb)

This course has been prepared for ISAE Supaero OTSU Cloud, Big Data and ML module.

The end goal of this exercise is to build temporal statistics from several Seninel-2 L2A products accessed from an object storage. In order to do this, we'll read the products using (rio)Xarray with a Dask backend, directly from Google Cloud Storage, compute a NDSI over ten dates and plot snow cover evolution accross the period.

By doing this, we will learn the folowing things:

- How to access a Cloud storage and browse its objects,
- How to use rioxarray to access and load Satellite imagery,
- How to use Xarray Dataset class to build a complete timeseries dataset,
- How to chunk our data and use Dask to perform bigger than memory or distributed analysis over our entire dataset.


## This repository uses Conda and Binder in order to make content easily available

Access this Binder by clicking the blue badge above or at the following URL:

http://mybinder.org/v2/gh/guillaumeeb/supaero-otsu-course/HEAD?urlpath=lab/tree/ndsi.ipynb

## Install localy

Just use the following command:

```
conda env create -f environment.yml
```