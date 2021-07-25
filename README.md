# Genre Classification Pipeline

Machine learning pipeline for a random forest classification model that classifies songs into its appropriate genre.

The repo uses MLflow and hydra to manage the parameters and pipeline components. Weights and Biases is used for artifact versioning.

## Using the repo

You will need to have `MLflow` and `wandb` installed in your virtual environment and have logged in to `wandb`.

```bash
    mlflow run <url-of-github-repo> -v <version> [-P ...]
```

E.g.
```bash
    mlflow run https://github.com/ashrielbrian/genre_classification.git -v 1.0.0  \
        -P hydra_options="main.project_name=remote_execution"
```

