# Building Fair AI models tutorial at PyData New York, 2018


###This tutorial uses an open source Python package named [AI Fairness 360 or AIF360](https://github.com/ibm/aif360). 

###Please visit the above site and follow instructions to install the package.

###Additionally, download datasets following instructions at [https://github.com/IBM/AIF360/tree/master/aif360/data](https://github.com/IBM/AIF360/tree/master/aif360/data)



### Alternatively, instructions are provided below for manually installing AIF360 and downloading datasets using Conda on Windows

Create and activate environment

```bash
conda create --name aif360 python=3.5
conda activate aif360
```



Clone AIF360 from GitHub:

```bash
git clone https://github.com/IBM/AIF360
```

Install R-essentials for downloading MEPS data

```bash
conda install -c r r-essentials
```

Download datasets and place under appropriate folders under AIF360/aif360/data/raw by cloning this repository (NOTE: clone at same level as AIF360) and running the belowmentioned notebooks in the root folder
          
```bash
git clone https://github.com/monindersingh/pydata2018_fairAI_models_tutorial.git
```
Change to the root folder and run

```bash
jupyter notebook pydata_datasets.ipynb
jupyter notebook pydata_meps_datasets.ipynb
```


Then, navigate to the root directory of the cloned AIF360 project and run:

```bash
pip install .
```



Finally, install the additional requirements as follows:

```bash
conda install ecos
pip install -r requirements.txt
```

