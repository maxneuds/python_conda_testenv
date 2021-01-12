# python_conda_testenv
Test environment for a conda controlled environment pipeline.

## Install

```bash
git clone git@github.com:maxneuds/python_conda_testenv.git
cd python_conda_testenv
conda create --name mathplot --file requirements.txt
conda activate mathplot
conda install ipykernel
python -m ipykernel install --user --name mathplot --display-name "mathplot"
```
## Update

```bash
conda list -e > requirements.txt
```

## Uninstall

```bash
conda activate notebook_env
jupyter kernelspec uninstall mathplot
conda remove --name mathplot --all
```
