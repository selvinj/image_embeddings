# image-embeddings
Using efficientnet to provide embeddings for retrieval.

Why this repo ? Embeddings are a widely used technique that is well known in scientific circles. But it seems to be underused and not very well known for most engineers. I want to show how easy it is to represent things as embeddings, and how many application this unlocks.

## Workflow
1. download some pictures
2. run inference on them to get embeddings
3. simple knn example, to understand what's the point : click on some pictures and see KNN

# Installation

## Prerequisites

Make sure you use `python>=3.6` and an up-to-date version of `pip` and
`setuptools`

    python --version
    pip install -U pip setuptools

It is recommended to install `image-embeddings` in a new virtual environment. For
example

    python3 -m venv image_embeddings_env
    source image_embeddings/bin/activate
    pip install -U pip setuptools
    pip install image_embeddings

## Using Pip

    pip install image-embeddings

## From Source

First, clone the `image-embeddings` repo on your local machine with

    git clone https://github.com/rom1504/image-embeddings.git
    cd image-embeddings
    make install

To install development tools and test requirements, run

    make install-dev

# Test

To run unit tests in your current environment, run

    make test

To run lint + unit tests in a fresh virtual environment,
run

    make venv-lint-test

# Lint

To run `black --check`:

    make lint

To auto-format the code using `black`

    make black

## Tasks

* [ ] simple downloader in python
* [ ] simple inference in python using https://github.com/qubvel/efficientnet
* [ ] build python basic knn example using https://github.com/facebookresearch/faiss
* [ ] build basic ui using lit element and some brute force knn to show what it does, put in github pages
* [ ] use to illustrate embeddings blogpost
