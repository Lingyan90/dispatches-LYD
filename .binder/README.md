# Run example notebooks in Binder

Binder (https://mybinder.org) provides a short-lived, temporary Linux cloud environment where Jupyter notebooks can be run without having to install any software locally.

## Quickstart

Click on this button to launch an environment pointing to the current `main` branch of this repository: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gmlc-dispatches/dispatches/HEAD)

## Limitations (IMPORTANT!)

### A Binder environment is temporary

A Binder environment is destroyed automatically after a few minutes of inactivity, which means that **any unsaved progress will be lost**. To avoid this, users should download a copy of a notebook file from the Binder environment to their local machine through the browser (in the Jupyter Lab file browser menu, right click on the notebook file > Download). For more information, see https://mybinder.readthedocs.io/en/latest/about/about.html#how-long-will-my-binder-session-last.

### Possible unavailability of the mybinder.org service

The mybinder.org service is an independent (i.e. unaffiliated with this project), general-purpose computational platform that is made available free-of-charge to the public. In our experience it has generally good uptime, however **outages (planned or otherwise) will occur** occasionaly.

Refer to the [Status page](https://https://mybinder.readthedocs.io/en/latest/about/status.html) and the additional resources listed there to access the most up-to-date information about the status of the service.

## Customization

Binder uses a Git repository hosted on e.g. GitHub to fetch the notebooks and create the runtime environment.
Users can specify a specific fork, branch, and Git ref (e.g. a particular commit hash), as well as the path to a particular directory or notebook file within the repository, that will be used
when first starting the environment.

These options can be specified interactively on [Binder's homepage](https://mybinder.org/), which will create a URL that can then be shared with others to generate a (separate) instance of the environment with the same repository settings.

Alternatively, the URL can be generated manually according to the following schema:

```txt
https://mybinder.org/v2/gh/<github-org-or-user-name>/<github-repo-name>/<git-ref>?labpath=<path-to-notebook>
```

Example: for a branch named `mybranch` belonging to `myuser`'s fork of this repository, pointing to the `dispatches/models/renewables_case/ConceptualDesignOptimization.ipynb` notebook file:

```txt
https://mybinder.org/v2/gh/myuser/dispatches/mybranch?labpath=dispatches/models/renewables_case/ConceptualDesignOptimization.ipynb
```
