# Dalil


## Requirements

- Python 3.12

#### Install Python using MiniConda

1) Download and install MiniConda from [here](https://docs.anaconda.com/free/miniconda/#quick-command-line-install)
2) Create a new environment using the following command:
```bash
$ conda create -n rag python=3.12
```
3) Activate the environment:
```bash
$ conda activate rag
```

### (Optional) Setup you command line interface for better readability

```bash
export PS1="\[\033[01;32m\]\u@\h:\w\n\[\033[00m\]\$ "
```



## Installation

### Install the required packages

```bash
$ git clone https://github.com/AhmedKamel200058/Dalil.git
$ Dalil
$ uv synch
```
#### if you not use uv can be download dependancies by using req.txt

```bash
$ pip install -r requirements.txt

```

### Setup the environment variables

```bash
$ cp .env.example .env
```

Set your environment variables in the `.env` file. Like `OPENAI_API_KEY` value.



## Run the FastAPI server (Development Mode)

```bash
$ uv run uvicorn dalil.main:app --reload --host 0.0.0.0 --port 8000
```