# IMPACT
IMPACT: Interpretable Microbial Phenotype Analysis via microbial Characteristic Traits

![](https://github.com/Wenze18/IMPACT/blob/main/IMPACT.png)

We present a framework that combines a feature engineering step to transform tabular ASV abundance data to sample wised image-format using functional microbial annotation databases, with a residual spatial attention transformer block architecture for phenotype classification. 

We find that our model delivers improved predictive accuracy performance across multiclass classification compared to similar methods. More importantly, our approach provides interpretable feature importance through image classification saliency methods. This enables the extraction of taxa markers (features) associated with a disease outcome but also their associated functional microbial traits and metabolites.


## Table of Contents

* [Installation](#Installation)
* [Usage](#Usage)
* [Citation](#Citation)


## Installation

To correctly use **IMPACT** via your local device, we suggest first create a conda environment by:

~~~shell
conda create -n <env> python=3.9
conda activate <env>
~~~

After entering an entire new virtue environment, the recommended way to install our package is:

~~~shell
pip install IMPACTBIOINFORMATICS
~~~
This commend would automatically download and install the lastest version (should be after 4.7) onto your local device.

Another alternative way to install the package is using the .tar file provided in this repo by:

~~~shell
pip install IMPACTBIOINFORMATICS-X.X.tar.gz
~~~

After this, validate the installation success in python by:

~~~shell
import impact
print(impact.__version__)
~~~

## Usage




## Citation

If you find our codes useful, please consider citing our work:

~~~bibtex
@article{IMPACT,
  title={IMPACT: Interpretable Microbial Phenotype Analysis via microbial Characteristic Traits},
  author={},
  journal={},
  year={2024},
}
~~~
