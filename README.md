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
- **Environment Names**:  
  Conda environment names must be **unique**. You cannot have multiple environments with the same name on the same system.

- **Location**:  
  Conda environments are stored **separately** from your project folder. They exist within the `conda` installation directory, not in the project directory itself. This helps keep environments isolated and ensures you can reuse them across projects.




<br><br>

## Delete environment
```shell
conda deactivate
conda env remove -n myenv
```











<br><br>
<br><br>
___
___
<br><br>
<br><br>


# FAQ / Error

## Installed dependencies not detected VS Code
- https://stackoverflow.com/questions/71113116/modulenotfounderror-no-module-named-fastapi
- Try restrat VS Code Window or/and The solution was, in VSCODE: CTRL + SHIFT + P then Python:select interpreter and choose the version of python linked to your environment.
