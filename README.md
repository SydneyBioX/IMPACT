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
~~~
If no error occurs, then IMPACT has been sucessfully installed.

## Usage

There are two main functions implemented within IMPACT, "train()" and "predict()".

Function train(input_file, metabolites_file, isize, check_feature_importance) could help user to train a Phenotype Prediction Model and analysis the data via microbial characteristic traits. It has 4 arguements, respectively are:

~~~
--input_file: should be a str. The absolute path of the input file,
              should be a .csv file, containing a matirx of normalized data.
              Each line represents a patient while each column represent a type of bacteria.
              Note that the last line is phylum information of all measured bacterias.

--metabolites_file: should be a str. The absolute path of the metabolites file,
              should be a .csv file, containing a matirx of normalized data.
              Each line represents a type of bacteria while each column represent a kind of metabolite. 
              IF you DO NOT have your customized one, please use the file provided in this repo.

--isize: should be an int. Default value is set to 60, determined by
              hyper-parameter searching via a couple cross validation,
              This arguement represents the image size of transformed input data.

--check_feature_importance: should be a bool. Default is set as Ture.
              This is the switch to draw the saliency plot.
              Important for microbial characteristic trait analysis.
              If True, would produce a .png file like following.
~~~
![](https://github.com/Wenze18/IMPACT/blob/main/saliency.png)


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
