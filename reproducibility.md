---
layout: page
title: Reproducibility
---

This page is a collection of reproducible research materials designed for educational use!

Contact: Fraida Fund (ffund@nyu.edu)

This material is based upon work supported by the National Science Foundation under Grant No. 2226408.

### Machine Learning

* [Deep Neural Nets: 33 years ago and 33 years from now](https://github.com/teaching-on-testbeds/deep-nets-reproducing/) (Fraida Fund). In this sequence of experiments, we will reproduce a result from machine learning from 1989 - a paper that is possibly the earliest real-world application of a neural network trained end-to-end with backpropagation. (In earlier neural networks, some weights were actually hand-tuned!) We'll go a few steps further, though - after reproducing the results of the original paper, we'll get to use some modern 'tricks' to try and improve the performance of the model without changing its underlying structure (i.e. no change in inference time!)

* [Reproducing "Characterization of Term and Preterm Deliveries using Electrohysterograms Signatures"](https://github.com/shaivimalik/medicine_preprocessing-on-entire-dataset) (Shaivi Malik, 2024 Summer of Reproducibility). In this sequence of notebooks, we will reproduce the results from Khan et al, "Characterization of Term and Preterm Deliveries using Electrohysterograms Signatures," which predicts pre-term birth based on raw EHG signals from pregnant women. However, it turns out that the reported 95.5% accuracy is much higher than we would achieve on new EHG signals because of data leakage in the oversampling process. We repeat the original pre-term birth prediction, but without the data leakage error, and show that the true performance of the model is much less.

* [Reproducing "Identification of COVID-19 samples from chest X-Ray images using deep learning: A comparison of transfer learning approaches"](https://github.com/shaivimalik/covid_illegitimate_features) (Shaivi Malik, 2024 Summer of Reproducibility). In this series of notebooks we reproduce a result published in Rahaman et al. "Identification of COVID-19 samples from chest X-Ray images using deep learning: A comparison of transfer learning approaches". However, a significant demographic inconsistency exists: normal and pneumonia chest X-ray images are from pediatric patients, while COVID-19 chest X-ray images are from adults. This allows the model to achieve high accuracy by learning features that are not clinically relevant. When we use datasets containing adult chest X-ray images, the model performance is much lower.

* [Reproducing "Skin Cancer Classification Using Inception Network and Transfer Learning"](https://github.com/kyrillosishak/re-SkinCancer) (Kyrillos Ishak, 2024 Summer of Reproducibility). In this series of notebooks, we will explore a result from Benedetti et al., "Skin Cancer Classification Using Inception Network and Transfer Learning", where the authors use transfer learning on a pretrained convolutional neural network to classify skin lesions in dermatoscopic images from HAM10000 (Human Against Machine with 10000 training images) dataset.  However, this example has a kind of data leakage where there are duplicate images of the same lesion in both the training set and the validation set that is used to evaluate model performance.  We repeat the original work, but with a correct evaluation - making sure that there are no duplicate images in the training and validation sets - and see that the original evaluation is overly optimistic.


* [Reproducing "An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale"](https://github.com/teaching-on-testbeds/re_vit) (Mohamed Saeed, 2023 Summer of Reproducibility). The paper "An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale" by Dosovitskiy et al. introduces a novel way of applying the transformer architecture, which was originally designed for natural language processing, to image recognition tasks. We introduce and explain the problem and the claims of the original paper, determine which claims can be tested using the available data and models, use the code and functions provided by the authors to test each claim, and evaluate the reproducibility of the research.

* [Reproducing "Warm-Starting Neural Network Training"](https://github.com/teaching-on-testbeds/re_warm_start_nn) (Mohamed Saeed, 2023 Summer of Reproducibility).  In this project, we consider  "On Warm-Starting Neural Network Training" by Jordan T. Ash and Ryan P. Adam, which investigates the problem of training neural networks on incremental data and shows that warm-starting often leads to worse generalization performance than random initialization, even though the training losses are similar. We introduce and explain the problem and the claims of the original paper, determine which claims can be tested using the available data and models, use the code and functions provided by the authors to test each claim, and evaluate the reproducibility of the research.








