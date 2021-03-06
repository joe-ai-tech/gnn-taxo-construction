# Graph2Taxo

This is a PyTorch implementation of the paper "Taxonomy Construction of Unseen Domains via Graph-based Cross-Domain Knowledge Transfer".

Published in [ACL 2020](https://acl2020.org/). 

## Installation

Install PyTorch using the official website or Anaconda.

## Initializing Git submodules. 

After cloning the repo, if you need to process the data, please use the command `git submodule update` to initialize the dependent submodules. This will clone [TaxoRL](https://github.com/morningmoni/TaxoRL) and [TAXI](https://github.com/uhh-lt/taxi/) projects that are used to reproduce data from existing experiments. 

    git submodule update

## Train model

### Dataset

TAXI data is given in the "data/TAXI_dataset" folder. Data from TaxoRL paper is given in the "data/TaxoRL_dataset" folder.

When you process the data, you can run:

    python preprocess.py

### Train model

When you train the model, you can run:

    python train.py


## Design your own model

You can directly modify the GRAPH2TAXO model in the "models.py" file.

## Acknowledgments
[GCN](https://github.com/tkipf/gcn), [TaxoRL](https://github.com/morningmoni/TaxoRL), [TAXI](https://github.com/uhh-lt/taxi) and [SACN](https://github.com/JD-AI-Research-Silicon-Valley/SACN).


