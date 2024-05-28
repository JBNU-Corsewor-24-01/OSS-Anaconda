# OSS-Anaconda


# Anaconda Python Environments Setup Project

## Introduction
This project demonstrates how to set up multiple Python environments using Anaconda. We will install Python versions 2.7, 3.6, 3.8, and 3.10, and create virtual environments for each version. Finally, we'll show how to list all available environments.

## Prerequisites
- Download and install [Anaconda](https://www.anaconda.com/products/distribution).

## Installation Guide

### Step 1: Install Anaconda
1. Download the Anaconda installer for your operating system from the [official website](https://www.anaconda.com/products/distribution).
2. Run the installer and follow the on-screen instructions.
3. After installation, open the Anaconda Prompt (or your preferred terminal).

### Step 2: Create Virtual Environments for Different Python Versions
Run the following commands in the Anaconda Prompt to create virtual environments for Python 2.7, 3.6, 3.8, and 3.10:

```bash
# Create a virtual environment with Python 2.7
conda create -n py27 python=2.7

# Create a virtual environment with Python 3.6
conda create -n py36 python=3.6

# Create a virtual environment with Python 3.8
conda create -n py38 python=3.8

# Create a virtual environment with Python 3.10
conda create -n py310 python=3.10
```

### Step 3: Activate and Deactivate Environments
You can activate any of the created environments using the following commands:

```bash
# Activate Python 2.7 environment
conda activate py27

# Deactivate the current environment
conda deactivate

# Activate Python 3.6 environment
conda activate py36

# Activate Python 3.8 environment
conda activate py38

# Activate Python 3.10 environment
conda activate py310
```

### Step 4: List All Available Environments
To list all the environments created, run:

```bash
conda env list
```

Or you can use the shorthand:

```bash
conda info --envs
```

## Usage
- Use the appropriate `conda activate <env_name>` command to switch between different Python environments.
- Use `conda deactivate` to exit the current environment.

## Troubleshooting
- If you encounter issues with creating environments, ensure that Anaconda is properly installed and that your PATH variable is correctly set.
- For issues related to package installations or conflicts, consider updating Conda or using the `--override-channels` flag with `conda create`.

## Conclusion
By following this guide, you can manage multiple Python versions on your system using Anaconda. This setup is particularly useful for testing code compatibility across different Python versions and for working on multiple projects with varying dependencies.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
