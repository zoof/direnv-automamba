# direnv-automamba

Use `direnv` to automatically activate mamba environment. Assumes that micromamba executable is in the $PATH.

Tested with `fish` shell:
* requires `.envrc` file in the directory of activations with format:<br>
```
layout mamba [environment-name]
```
* environment.yml file activation not working