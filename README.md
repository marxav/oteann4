# OTEANN 

This repository is the official implementation of [OTEANN: Estimating the Transparency of Orthographies with an Artificial Neural Network](https://arxiv.org/abs/1912.13321v4).

## Requirements

* Require Ubuntu 18.04, Python 3.6+.

* Download files on your machine
  * git clone https://github.com/marxav/oteann4.git

* Go to the oteann4 main directory
  * cd oteann4 

* Create a virtual environment
  * python3 -m venv oteann 

* Activate virtual environment
  * source oteann/bin/activate

* Load the python librairies needed for OTEANN (e.g. numpy, pandas, torch...) from the requirements file
  * python -m pip install -r requirements.txt
  
* Extract the subdatasets (required local free spacesize=334Mo)
  * python extract_subdatasets.py

## Evaluation and Training

In order to run this code, you need to:
* Run the [oteann.ipynb](oteann.ipynb) in order to create the ANN model, train it, test it and display the results of the paper.

## Results

OTEANN achieves the following performance:

|orthography| write score| read score |
|-----------|------------|------------|
|    ent    | 99.6 ± 0.3 | 99.8 ± 0.1 |
|    eno    | 00.0 ± 0.0 | 00.0 ± 0.0 |
|    ar     | 84.3 ± 0.8 | 99.4 ± 0.3 |
|    br     | 80.6 ± 0.6 | 77.2 ± 1.6 |
|    de     | 69.1 ± 1.0 | 78.0 ± 1.5 |
|    en     | 36.1 ± 1.5 | 31.1 ± 1.3 |
|    eo     | 99.3 ± 0.2 | 99.7 ± 0.1 |
|    es     | 66.9 ± 2.0 | 85.3 ± 1.3 |
|    fi     | 97.7 ± 0.3 | 92.3 ± 0.8 |
|    fr     | 28.0 ± 1.4 | 79.6 ± 1.7 |
|    fro    | 99.0 ± 0.3 | 89.7 ± 1.1 |
|    it     | 94.5 ± 0.8 | 71.6 ± 0.9 |
|    ko     | 81.9 ± 1.0 | 97.5 ± 0.5 |
|    nl     | 72.9 ± 1.7 | 55.7 ± 2.2 |
|    pt     | 75.8 ± 1.0 | 82.4 ± 0.9 |
|    ru     | 41.3 ± 1.6 | 97.2 ± 0.5 |
|    sh     | 99.2 ± 0.3 | 99.3 ± 0.3 |
|    tr     | 95.4 ± 0.7 | 95.9 ± 0.6 |
|    zh     | 19.9 ± 1.4 | 78.7 ± 0.9 |

## License

OTEANN uses minGTPT (https://github.com/karpathy/minGPT) which is released under the MIT licence.

## Citation
This code was used for the following paper:
```bibtex
@misc{marjou2020oteann,
      title={OTEANN: Estimating the Transparency of Orthographies with an Artificial Neural Network}, 
      author={Xavier Marjou},
      year={2021},
      eprint={1912.13321v4},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
