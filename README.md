# direnv-automamba

Use `direnv` to automatically activate a mamba environment. Assumes that micromamba executable is in the $PATH. The contents of `.direnvrc` goes in either `~/.direnvrc` or `~/direnv/direnvrc`.

Tested with `bash` and `fish` shells.

Requires `.envrc` file in the directory where mamba is to be activated and should contain:<br>

```
layout mamba [environment-name]
```

* If `environment-name` is supplied then `environment-name` is activated.
* If `environment-name` is not supplied and `environment.yml` exists and contains `name:` then the environment specified is activated.
* If `environment-name` is not supplied and `environment.yml` does not exist or exists but does not contain `name:` then the `base` environment is activated.
