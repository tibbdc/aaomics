# aaomics

Omics data analysis reveals the system-level constraint on cellular amino acid composition

## Software

To create a stand-alone environment named aaomics with Python 3 and all the required package versions (especially for cobrapy is also available), run the following code:

```shell
$ conda create -n aaomics python=3
```
```shell
$ conda activate aaomics
```
```shell
$ pip install ipykernel  
$ python -m ipykernel install --user --name aaomics --display-name "aaomics"  
$ pip install pandas
$ pip install Bio
$ pip install matplotlib
$ pip install seaborn
$ pip install cobra
```
  You can read more about using conda environments in the [Managing Environments](http://conda.pydata.org/docs/using/envs.html) section of the conda documentation. 

## Steps to reproduce the main analysis in the publication

#### 1.analysis_workflow.ipynb  
>+ Data Acquisition  
>+ Get protein MW/Sequence corresponding to gene id using uniprot API    
>+ Get amino acid composiotion from protein sequence  
>+ Amino acid composition condsider protein sequence   
>+ Amino acids composition of each protein (g / g protein) consider expression level under different conditions  
>+ Amino acids composition of each condaition (g / g total protein) consider expression level  

#### 2.draw_figure_in_article.ipynb  
>+ The mass distribution of each AA in per unit mass of different proteins  
>+ The mass ratio distribution of different proteins in per unit mass of total protein (only the pro-teins with a mean mass ratio among the top 50 are displayed)  
>+ The mass distribution of each AA per unit mass of total protein  
>+ Distribution of the mass ratio of twenty AAs per unit mass of total protein in different species  
