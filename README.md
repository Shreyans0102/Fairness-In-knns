Fair Information Bottleneck: Mitigating Unfairness in kNN Classifiers

This repository contains the project report and the implementation code for our work on reducing bias in kNN classifiers through a fairness-aware embedding approach.
Overview

    Objective:
    Develop a novel embedding method based on a modified Variational Autoencoder (VAE) loss function to reduce sensitive demographic information from datasets. The goal is to mitigate discriminatory predictions made by kNN classifiers while preserving model accuracy.

    Approach:
    We adjust the traditional information bottleneck loss function by incorporating a fairness component. This modification compresses sensitive attributes while retaining task-relevant information. We evaluate our method against several baselines:
        Raw data with kNN.
        Fairness-agnostic autoencoder embeddings.
        Fair representation embeddings (as introduced by Zemel et al.).

    Datasets:
        German Credit Dataset: Binary classification to assess credit risk with sensitive features (e.g., gender).
        Adult Income Dataset: Binary prediction task determining if income exceeds $50K, with age as the sensitive attribute.
        
        
        Citations
        
        
@InProceedings{pmlr-v28-zemel13,
  title = 	 {Learning Fair Representations},
  author = 	 {Zemel, Rich and Wu, Yu and Swersky, Kevin and Pitassi, Toni and Dwork, Cynthia},
  booktitle = 	 {Proceedings of the 30th International Conference on Machine Learning},
  pages = 	 {325--333},
  year = 	 {2013},
  editor = 	 {Dasgupta, Sanjoy and McAllester, David},
  volume = 	 {28},
  number =       {3},
  series = 	 {Proceedings of Machine Learning Research},
  address = 	 {Atlanta, Georgia, USA},
  month = 	 {17--19 Jun},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v28/zemel13.pdf},
  url = 	 {https://proceedings.mlr.press/v28/zemel13.html},
  abstract = 	 {We propose a learning algorithm for fair classification that achieves both group fairness (the proportion of members in a protected group receiving positive classification is identical to the proportion in the population as a  whole), and individual fairness (similar individuals should be treated similarly).  We formulate fairness as an optimization problem of finding a  good representation of the data with two competing goals: to encode the data as well as possible, while simultaneously obfuscating any information about membership in the protected group.  We show positive results of our algorithm relative to other known techniques, on three datasets.  Moreover, we demonstrate several advantages to our approach.  First, our intermediate representation can be used for other classification tasks (i.e., transfer  learning is possible); secondly, we take a step toward learning a distance metric which can find important dimensions of the data for classification.}
}

