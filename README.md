# conda-cheat



## Miniconda

<br><br>

### Install
- https://docs.anaconda.com/miniconda/install/#quick-command-line-install
```
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh

source ~/miniconda3/bin/activate

conda init --all
```





<br><br>
<br><br>
___
___
<br><br>
<br><br>

# Environment

## Create environment
```shell
# Create a new conda environment with Python 3.10
conda create -n myenv python=3.10

# Activate the environment
conda activate myenv

# Install dependencies
conda install pytorch transformers -c conda-forge
```



<br><br>

## Delete environment
```shell
conda deactivate
conda env remove -n myenv
```
