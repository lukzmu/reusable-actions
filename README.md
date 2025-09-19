# Reusable Actions

This repository holds a set of reusable actions for my Python projects. It is licensed under the [MIT License](LICENSE), so feel free to do whatever you want with it. Any issues you encounter... that is a *"you problem"*.

## How to use?

You want to select a specific action in your workflow. Be sure to see the `name` and the `version` you are interested in. Versions are defined by **tags**. So for example, to run the first release of the `setup-python` action, you should do the following:

```
steps:
    - uses: lukzmu/reusable-actions/setup-python@v1
      with:
        python-version: "3.14"
        main-module: "my_source_module"
```

## Available actions:

| **Action**                                    | **Description**                                         |
|-----------------------------------------------|---------------------------------------------------------|
| [setup-python](setup-python/action.yml)       | Sets up some handy things to use the uv package manager |
| [code-quality](code-quality/action.yml)       | Check ruff, mypy, tests and publish coverage reports    |
| [pelican-publish](pelican-publish/action.yml) | Publish pelican site to GitHub Pages                    |
