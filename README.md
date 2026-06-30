# Software Development Project (C1PP2B_2026) Autumn 2026

This is the repository for the Software Development Project (Autumn 2026) course at Borås University.

The course schedule can be found on [Kronox](https://schema.hb.se/setup/jsp/Schema.jsp?sprak=En&sokMedAND=false&intervallAntal=6&startDatum=2025-11-10&intervallTyp=m&resurser=k.C1PP2B-20252-I30H5-) and the course material can be found on [Canvas](https://hb.instructure.com/courses/10079).

## Delopment Environment Setup

First, make sure you have installed Visual Studio Code, Git, and Miniconda on your computer.

### Software

Install the following software on your computer:

- [Visual Studio Code](https://code.visualstudio.com)
- [Git](https://git-scm.com/downloads)
- [Miniconda](https://docs.anaconda.com/miniconda/install/#quick-command-line-install)
- [Python](https://www.python.org) (optional) - comes pre-installed on Linux and Mac

### Verify the Software Installation

Verify the software has been successfully installed, by opening a terminal and issuing the following commands (each command should print out a version):

- `code --version`
- `git --version`
- `conda --version`

If you don't see the print-out of a version for a specific tool, make sure the path to your tool's folder has been added to your [`PATH` environment variable](https://gist.github.com/nex3/c395b2f8fd4b02068be37c961301caa7).

### Visual Studio Code (VSCode) Extensions

Then install the necessary Visual Studio Code Extensions by executing the commands below in your terminal:

- `code --install-extension ms-toolsai.jupyter`
- `code --install-extension ms-python.python`
- `code --install-extension 42crunch.vscode-openapi --force`
- `code --install-extension arjun.swagger-viewer --force`

### Accounts

Create a GitHub account (if you don't already have one):

- Visit the [GitHub](https://github.com) web site and [Sign up](https://github.com/signup) for an account.

## Course Repository

When you have installed the software above, open a terminal and clone the GitHub repository [C1PP2B_2026](https://github.com/paga-hb/C1PP2B_2026.git) to your computer, and create a Python environment:

- `git clone https://github.com/paga-hb/C1PP2B_2026.git dev`
- `cd dev`
- `conda create -y -p ./.conda python=3.12`
- `conda activate ./.conda`
- `python -m pip install --upgrade pip`
- `pip install ipykernel pylint`
- `pip install numpy pandas matplotlib seaborn plotly scikit-learn`
- `pip install torch`
- `pip install "tensorflow[and-cuda]"`
- `pip install chromadb weaviate-client requests`
- `pip install pyodbc sqlalchemy`

## Open the First Workshop Notebook

Finally, make sure you are in the `dev` folder in your terminal, and open one of the notebook in Visual Studio Code, by issuing one of the command below:

- `code -g notebooks/flask.ipynb:0 .`
- `code -g notebooks/fastapi.ipynb:0 .`
- `code -g notebooks/rag.ipynb:0 .`
- `code -g notebooks/pt.ipynb:0 .`
- `code -g notebooks/tf.ipynb:0 .`

When the notebook opens in VSCode, click the text `Select Kernel` (in the top-right of the notebook), and choose `Python Environments... => conda (Python 3.12) .conda/bin/python`.

Now you can follow the instructions in the notebook.
