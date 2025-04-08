---
layout: page
title: Pattern recognition in remote sensing - exercises and datasets
---

A collection of exercises should be completed and reported **on time** until the end of semester. 
It does not matter what programming language are you using, but your results and reports will be evaluated.
Send your comprehensive reports via [Email](mailto:torabzadeh@basu.ac.ir).

* TOC
{:toc}

# Datasets
Passwords will be sent via lecture channels in Telegram or via Email.

## No.1: Agricultural region
This dataset includes remotely sensed imageries of an agricultural region in USA. The data are collected and regularly updated by USDA and distributed by [CSISS](https://nassgeodata.gmu.edu/CropScape/), George Mason University.

We need bellow parts for performing the exercises: 
1. Sentinel-2 MSI data: *Sentinel-2-MSI-for-Exercise-01.tif*
2. Landsat 9 OLI data: *Landsat-9-OLI-for-Exercise-01.tif*
3. Sentinel-1 SAR data: *Sentinel-1-SAR-for-Exercise-01.tif*
4. Classification results (2022): *CDL_2022_clip_20240408032210_1404219373.tif*
5. Classification keys: *Cropland Data Layer (CDL) Key.pdf*

You will find the datasets [here](https://mega.nz/file/NSNABJoR#YMxuvs6zjOB3XbCY5vqHds4L8krx-EWnsvYCvPe728w)

## No.2: Ekbatan Reservoir
This dataset includes time series of Landsat images over Ekbatan reservoir, Hamedan, Iran. 

It contains six images in PNG format, showing the reservoir water body changes from 2018 to 2023. An animation of changes was also added in GIF format.  

You will find the datasets [here](https://mega.nz/file/9Os3BSRa#K1Ph7IvrM8xkqaM80kmCr-XcKqJ4teFFfY1C2HLpk1I)

# Exercises
## 1. Covariance & Correlation

- Download Dataset No.1.
- Calculate covariance and correlation matrices for Sentinel-2 MSI, Sentinel-1-SAR and Landsat 9 OLI, separately.
- Calculate correlations between Sentinel-2 MSI bands and Sentinel-1-SAR bands. Write your conclusions.
- Calculate correlations between Sentinel-2 MSI bands and Landsat 9 OLI bands. Write is your conclusions.

## 2. Principal component analysis

- Download Dataset No.1.
- Calculate principal components for Sentinel-2 MSI, Sentinel-1-SAR and Landsat 9 OLI, separately.
- Indicate the most important PCs for each dataset and their influences.
- Create a false color composite from three first PCs and visually compare it with the RGB image, for each dataset.

## 3. PCA for change detection

- Download Dataset No.2.
- Select two different years (e.g. 2017 and 2018) and enhance the changes in the water body using principal components analysis.
- compute the changed area for all years, relative to 2017 and create a clear chart.
- How do you confirm your results with the annual precipitation reports?
- How can separate changes in fire burned rangelands between 2022 and 2023?

## 4. Maximum likelihood classification

- We are going to classify the Landsat 9 OLI image to three classes, i.e vegetation, bare soil and water bodies.
- extract enough number of proper pixels in each class from the image and save them into a table (or text file).
- train maximum likelihood classifier using the sample data.
- label all pixels and produce thematic map (or landcover map).

## 5. Minimum distance classification

- Change your classifier to Minimum Distance and repeat all steps (in exercise 4)
- Visually compare your results with the outputs from maximum likelihood classifiers.
- Send your reports.

## 6. SVM classification

- Change your classifier to Support vector machine and repeat all steps (in exercise 4)
- Visually compare your results with the outputs from maximum likelihood and minimum distance classifiers.
- Send your reports.

