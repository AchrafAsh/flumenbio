# flumenbio
A fake biotech startup that have everything from a real one, except it's fake.

### Drug Discovery
3 tasks:

1. Predicting molecule properties
2. De Novo drug design
3. Predicting molecule-target activity

### Datasets
- QM9: Predicting molecular properties (load with Pytorch Geometric | https://www.kaggle.com/zaharch/quantum-machine-9-qm9)
- PPI: Predicting protein-protein interaction (load with Pytorch Geometric)
- UniProt: (protein, gene, disease, ...) https://www.uniprot.org
- Tox21: structure-activity relationship


### Papers

#### Molecule Properties


#### Drug Design
![](https://pocket-image-cache.com//filters:format(jpg):extract_focal()/https%3A%2F%2Fmiro.medium.com%2Fmax%2F1400%2F1*kRVBrKwcxITa8PRJFtyqLg.png)

- [Automatic Chemical Design Using a Data-Driven Continuous Representation of Molecules](https://pubs.acs.org/doi/full/10.1021/acscentsci.7b00572)
- [Grammar Variational Autoencoder](https://arxiv.org/pdf/1703.01925.pdf)
- [Objective-Reinforced Generative Adversarial Networks (ORGAN) for Sequence Generation Models](https://arxiv.org/pdf/1705.10843.pdf)
- [Junction Tree Variational Autoencoder for Molecular Graph Generation](https://arxiv.org/abs/1802.04364)
- [Augmenting Genetic Algorithms with Deep Neural Networks for Exploring the Chemical Space](https://arxiv.org/abs/1909.11655) (uses QM9 dataset, Genetic Algorithm and a NN as discriminator)

#### Molecule-Target Activity (QSAR?)
- [PADME: A Deep Learning-based Framework for Drug-Target Interaction Prediction](https://arxiv.org/abs/1807.09741)
- [DeepCCI: End-to-end Deep Learning for Chemical-Chemical Interaction Prediction](https://arxiv.org/abs/1704.08432)
- [Protein–Ligand Scoring with Convolutional Neural Networks](https://pubs.acs.org/doi/10.1021/acs.jcim.6b00740)


### Baselines:
- Molecular properties: Graph Convolutional Network trained on QM9
- Drug Design: two headed generator - add edge or node / attribute of the added component
- Drug-Target activity: 
