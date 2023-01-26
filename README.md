# ATFM regulation for specific Traffic Volumes

Repository part of the release provided to EUROCONTROL as part of my PhD. It 
contains the most relevant code developed and used during the PhD.

**NOTES:** 
> 1. No all the proof of concept and models used are included. 
> 2. The code is provided
as it is, without any guarantee on the functionalities nor in he reproducibility of 
the results published.


# Summary

This repository partially contains the code developed to train machine learning (ML)
to predict **ATFM regulations at the traffic volume level**. 

# Content

It contains **three types of ML models**:
* RNN using scalar variables
* CNN using images
* Hybrid which contains the combination of the previous RNN and CNN

# Usage

To run the previous models is necessary an environment with the libraries specified
in:
> requirements/atfm_tv.yml

# Architecture

* data/
  * input_data/ \
    -> Must contain the raw data to compute the input features 
  * input_features/ \
    -> Contains the pre-computed features
* libs/
* models/ \
  -> Contain pre-trained models for each supported case study
* notebooks/
  * RNN/
  * CNN/
  * Hybrid/
* requirements/
  * atfm_tv.yml \
    -> Requirement to the train/test/run the ML models
  * web_application.yml \
    -> Requirements top run the web application based on DJANGO
  * C++.yml \
    -> Requirements necessary to convert and test the ML models using C++