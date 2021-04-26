# **Guitar Effects Classifications**

![](img/pedals.jpg)

## **Overview**

This project implements a classifier system able to predict the audio effects used in recordings of electric guitar focusing in particular on distinguishing clean (no FX), distortion, and tremolo signals. 

The audio dataset is the [IDMT-SMT-Audio-Effects database](https://www.idmt.fraunhofer.de/en/business_units/m2d/smt/audio_effects.html), which is a large dataset for automatic detection of audio effects in recordings of electric guitar and bass and related signal processing.

To develop the classification algorithm, the following features are considered: 

- Mel-frequency cepstral coefficients (MFCCs) 
- Total harmonic distortion (THDN)
- Envelope Flatness
- Root Mean Square Energy (RMSE) 
- Spectral Centroid
- Spectral Bandwidth 
- Spectral Flatness 
- Spectral Rolloff
- Zero-Crossing Rate

Then they are analysed using the SelectKBest function from the scikit-learn library, which selects features according to the k highest scores. This ensures that only the most effective features are considered in the classifier. 

Two classification approaches are studied here:

- Supervised learning with support vector machines (SVMs) from scikit-learn library.
- Sequential neural network approach based on the tensorflow library. 

## **Classification Results**
![](img/svmcm.png)
![](img/nncm.png)



## **Report with models and results**
[Report](https://docs.google.com/document/d/1m-M3qP3C9z6Qg7EcXej9O9Hzm-puHk-ThQ6Iwsc-UcY/edit?usp=sharing)
