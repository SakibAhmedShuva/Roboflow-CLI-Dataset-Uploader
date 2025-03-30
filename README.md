# Roboflow CLI Dataset Uploader

A simple utility script for uploading and managing datasets using the Roboflow Command Line Interface.

## Overview

This repository contains a script to help you:
1. Install the Roboflow CLI
2. Authenticate with your Roboflow account
3. Import datasets for computer vision tasks using Roboflow's command line tools

## Prerequisites

- Python 3.6+
- Google Colab (recommended) or Jupyter Notebook environment
- Roboflow account (free signup at [roboflow.com](https://roboflow.com))

## Usage

Three main steps:

### 1. Install Roboflow CLI

```python
!pip install roboflow
```

### 2. Authenticate with Roboflow CLI

```python
!roboflow login
# log in to: https://app.roboflow.com/auth-cli
# copy the authentication code
# paste it in the notebook field
```

### 3. Import a Dataset with Roboflow CLI

```python
!roboflow import -w workspace-name -p project-name /path/to/dataset
```

This imports the dataset to your specified workspace and project using the Roboflow CLI.

## Example

The included example imports a YOLO-formatted dataset to a workspace called "damage-sverity" and a project called "high-school-it":

```python
!roboflow import -w damage-sverity -p high-school-it /content/damage-yolo-29-2-1-25-augmented
```

## Additional Roboflow CLI Commands

The Roboflow CLI offers many more commands for dataset management:
- Dataset versioning
- Model training
- Deployment
- Inference

Check the [official Roboflow documentation](https://docs.roboflow.com/cli) for more information.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
