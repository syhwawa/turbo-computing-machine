
# Installation

## Setting up a user environment

As a `yuhao_python_template_trial` user, it is easiest to install using the [mamba](https://mamba.readthedocs.io/en/latest/index.html) package manager, as follows:


1. Install mamba with the [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge) executable for your operating system.
2. Open the command line (or the "miniforge prompt" in Windows).

3. mamba create -n yuhao_python_template_trial -c conda-forge -c syhwawa yuhao_python_template_trial
4. Activate the yuhao_python_template_trial mamba environment: `mamba activate yuhao_python_template_trial`


All together:

--8<-- "README.md:docs-install-user"
### Running the example notebooks
If you have followed the non-developer installation instructions above, you will need to install `jupyter` into your `yuhao_python_template_trial` environment to run the [example notebooks](https://github.com/syhwawa/yuhao_python_template_trial/tree/main/examples):

``` shell
mamba install -n yuhao_python_template_trial jupyter
```

With Jupyter installed, it's easiest to then add the environment as a jupyter kernel: 

``` shell
mamba activate yuhao_python_template_trial
ipython kernel install --user --name=yuhao_python_template_trial
jupyter notebook
```

### Choosing a different environment name
If you would like to use a different name to `yuhao_python_template_trial` for your mamba environment, the installation becomes (where `[my-env-name]` is your preferred name for the environment):

``` shell
mamba create -n [my-env-name] -c conda-forge --file requirements/base.txt
mamba activate [my-env-name]
ipython kernel install --user --name=[my-env-name]
```
## Setting up a development environment

The install instructions are slightly different to create a development environment compared to a user environment:

--8<-- "README.md:docs-install-dev"

For more detailed installation instructions specific to developing the yuhao_python_template_trial codebase, see our [development documentation][setting-up-a-development-environment].
