# Contributor's Guide

## Setting up dev environment

We have individual uv environments for each package. To start, sync dependencies with the following command:

```sh
uv sync
```

## Run tests

```
uv run --group tests pytest tests/
```

To run a single test file, pass its path, for example `uv run --group tests pytest tests/databricks_ai_bridge/utils/test_vector_search.py`.

## Run Type Checker


In each project directory, run

```
uv run ty check
```

### Build API docs

See the documentation in docs/README.md for how to build docs. When releasing a new wheel, please send a pull request to change the API reference published in [docs-api-ref](https://github.com/databricks-eng/docs-api-ref/tree/main/content-publish/python/databricks-agents).
