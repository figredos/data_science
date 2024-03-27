# Environment setup

Once the machine learning and data science [framework](/TEXT_FILES/framework.md) has been established, the next step is to match tools to the steps in the framework. This may seem simple at first, but given the amount of tools it may seem cumbersome at first, but there are programs like Anaconda, MiniConda, and Conda that help manage all of these tools.

- [Environment setup](#environment-setup)
  - [Anaconda, MiniConda, Conda](#anaconda-miniconda-conda)
  - [Setup](#setup)
    - [Download](#download)
    - [Conda environment](#conda-environment)

## Anaconda, MiniConda, Conda

Anaconda and MiniConda are software distributions, that come with many of the tools needed to practice machine learning and data science. The big difference between them is that Anaconda is a full featured distribution of Python and data science. When installed comes with the Conda package manager, Python, hundreds of popular data science packages, and the Anaconda navigator. This is a more beginner friendly tool, for people who want a comprehensive environment with pre-installed tools, and who prefer a GUI for managing packages and environments. This however comes with its downside, given that Anaconda pre-installs so many tools and packages, most of them go unnoticed and unused by most people, and takes around 3Gb of space.

This is where MiniConda comes in. Unlike Anaconda, MiniConda is a minimal installer for conda, being much smaller, only taking up about 200Mb of storage space, and comes with fewer pre-installed tools. These tools include, the Conda package manager, Python, and a few essential packages.

Both of these versions though, come with the conda package manager, as previously mentioned. Conda is an open source package and environment manager specifically designed to address challenges faced in Data Science. It creates isolated environments where you can have different versions of Python and packages installed without affecting other projects. This is crucial to avoid conflicts between different projects requiring different dependencies.

The projects developed in this repo can be easily set up by only using MiniConda

## Setup

### Download

The first step would be to download MiniConda. This can be done by following the steps in this [link](https://docs.anaconda.com/free/miniconda/).

### Conda environment

Now that MiniConda has been installed, the next step is to create a conda environment. A conda environment is a self-contained directory that holds a specific collection of Python packages and their dependencies. It essentially isolates your project's dependencies from other projects or the system-wide Python installation.

To create a conda environment, open the terminal and enter the following commands:

1- Create the environment

```bash
conda create --prefix .<environment name> <environment path>
```

This begins the process of using conda. After the `--prefix` flag, pass the name of the environment, such as `env` followed by a period, like so `.env`.

After hitting enter, conda prompts `Proceed ([y]/n)?`, enter `y` and this will finish creating the environment.

As previously said, this starts the process, but to finish it the next step is crucial.

2- Activating environment

At the end of the generated message, conda informs that to activate the environment the following line of code needs to be executed:

```bash
conda activate <path to environment>
```

This does pretty much what it says, it switches the current environment conda is set in, to the environment present in the path.
