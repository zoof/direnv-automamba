# direnv-automamba

Use `direnv` to automatically activate a mamba environment. Assumes that micromamba executable is in the $PATH. The contents of `.direnvrc` goes in either `~/.direnvrc` or `~/direnv/direnvrc`.

Tested with `fish` shell:
* requires `.envrc` file in the directory where mamba is to be activated and should contain:<br>
```
layout mamba [environment-name]
```
where if no environment-name is supplied, the "base" environment will be activated.
* environment.yml file activation not working