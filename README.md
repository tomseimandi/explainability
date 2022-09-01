# Resources on XAI :

## General
- LIME : ["Why Should I Trust You?": Explaining the Predictions of Any Classifier](https://arxiv.org/abs/1602.04938)

## NLP :
- SHAP : [A Unified Approach to Interpreting Model Predictions](https://arxiv.org/abs/1705.07874)
- HEDGE : [Generating Hierarchical Explanations on Text Classification via Feature Interaction Detection](https://arxiv.org/abs/2004.02015)

## Time series :
- [Evaluation of time series by perturbating subsequences of the data](https://arxiv.org/abs/1909.07082)
  - Basic idea is to observe the drop in classification quality if perturbating the most important features both i) in isolation and ii) together with the following timestamps
- [Temporal Saliency Rescaling](https://arxiv.org/abs/1909.07082)
  - The main idea behind Temporal Saliency Rescaling is to divide feature importance attribution into two steps: first identify the important time steps and then within the time step the important feature. This should avoid the alleged issue that saliency methods tend to select a full time step as important although only a few features might be relevant
  - Unclear how the evaluation in fact works. Seems like the main idea is to just look at precision/recall for perturbed time series
- [Benchmarking Deep Learning Interpretability in Time Series Predictions](https://arxiv.org/pdf/2010.13924.pdf)
  - The main idea is a network architecture that allows to calculate a saliency map separately for the time and feature domain

## Imagery :
- [Grad-CAM: Why did you say that? Visual Explanations from Deep Networks via Gradient-based Localization](http://arxiv.org/abs/1610.02391)
- [Model-Agnostic Explanations](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16982)
- [Deep Inside Convolutional Networks: Visualising Image Classification Models and Saliency Maps](https://arxiv.org/abs/1312.6034)
- [Visualizing and Understanding Convolutional Networks](http://arxiv.org/abs/1311.2901)
- [Striving for Simplicity: The All Convolutional Net](https://arxiv.org/abs/1412.6806)
- [Learning Important Features Through Propagating Activation Differences](http://arxiv.org/abs/1704.02685)
- [On Pixel-Wise Explanations for Non-Linear Classifier Decisions by Layer-Wise Relevance Propagation](https://doi.org/10.1371/journal.pone.0130140)
- [SmoothGrad: removing noise by adding noise](http://arxiv.org/abs/1706.03825)
- [Expected gradients](https://arxiv.org/pdf/1906.10670.pdf)
- [Better Attributions through regions](https://arxiv.org/abs/1906.02825)
- [Visualizing the Impact of Feature Attribution Baselines](https://distill.pub/2020/attribution-baselines/)

## Evaluating a saliency map vs. evaluating a saliency method :
- [Representativity and consistency](https://arxiv.org/pdf/2009.04521.pdf)
- [Interpreting interpretations: Organizing attribution methods by criteria](https://arxiv.org/abs/2002.07985)
- [Sanity Checks for Saliency Maps](https://arxiv.org/abs/1810.03292)
- [On the (in)fidelity and sensitivity of explanations](https://arxiv.org/abs/1901.09392)
