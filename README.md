General information about what git hooks are and do: https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks  
Info about setting up pre-commit: https://pre-commit.com/ - most of the steps here are just following the instructions here.

## Client side checking
I.e. check your local changes when you run `git commit ...` command

### Install pre-commit python package
I will do this in a virtual environment
```shell script
python3 -m venv pc_venv
source pc_venv/bin/activate
pip install pre-commit
```

### Define a hook using a yaml file
THe file `pre-commit-config.yaml` for formatting python code using [black](https://pypi.org/project/black/).  
A `pyproject.toml` file is included that includes some configuration for black.

### Use pre-commit to set up the hooks
```shell script
source pc_venv/bin/activate
pre-commit install
pre-commit run --all-files
```

