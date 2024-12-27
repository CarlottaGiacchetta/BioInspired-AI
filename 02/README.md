### Requirements
0. We assume Anaconda is installed. One can install it according to its [installation page](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html).

1. Create a virtual environment

```shell
conda env create -f environment.yml
conda activate bio-ai
```

2. If you use Jupyter extension for VSCode, you may need to restart VSCode to select the new conda environment as a kernel

3. If you use Jupyter notebook local server, you need to add he new conda environment as a selectable kernel:
```shell
conda activate bio-ai
python -m ipykernel install --user --name bio-ai --display-name "Python (bio-ai)"
```

4. If you already have your virtual environment or do not fancy to use one, you can install the required libraries from the requirements file:
```shell
pip install -r requirements.txt
```