# Machine Learning Systems

Source: [CS249R Repo](https://github.com/harvard-edge/cs249r_book)

References : [TinyTorch](https://mlsysbook.ai/tinytorch/intro.html) | [MLSysBook](https://mlsysbook.ai/book/)

## Table of contents

## Introduction

This is a run at Harvard's CS 249R course on AI engineering.

**The premise**: you can't debug what you don't understand.

**The idea**: to understand machine learning systems by building them using a lightweight learning framework (TinyTorch vs PyTorch [complex production framework]).

**The objective**: to move from using machine learning to engineering machine learning systems.

## Setup

```bash
sudo apt update
sudo apt install python3.12-venv # I was missing this dependency
```

Install TinyTorch via [script](https://mlsysbook.ai/tinytorch/getting-started.html).

```terminal
[1/4] Downloading from GitHub...
✓ Downloaded TinyTorch (01fc7df)
[2/4] Creating Python environment...
✓ Created virtual environment using python3.12
[3/4] Installing dependencies...
✓ Installed dependencies
[4/4] Verifying installation...
✓ Verified tito CLI

✓ Tiny🔥Torch installed successfully!
```

```bash
tito --version # Tiny🔥Torch v0.1.7
```

```bash
tito system update 
tito system health
tito module status # Track progress
```

### Virtual environment

A virtual environment is like a lightweight container isolating Python's code and dependencies at the language level (project folder).

So that its operation doesn't interfere with the system or other projects.

`venv` is the Linux module to set up a virtual environment :

```bash
python3 -m venv your_env_name
source your_env_name/bin/activate # To activate it
```