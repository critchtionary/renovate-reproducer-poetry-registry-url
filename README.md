Repository to demonstrate issue with using Renovate, poetry and a custom registry URL

# Current behaviour

Github release for `containerbase/python-prebuild` is attempted to be installed from Python registry, resulting in an error:

```
DEBUG: Failed to look up github-releases package containerbase/python-prebuild (repository=example-repo, packageFile=pyproject.toml, dependency=containerbase/python-prebuild)
```

# Expected behaviour
Renovate should not attempt to obtain `containerbase/python-prebuild` from `registryUrls`.
