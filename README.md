# July Challenge: Image Classification

Submission for Tim Smith's Shokunin Challenge, July 2019.

## Installation

```
pip install -r requirements.txt
```

## Usage

```
jupyter notebook src/notebook.ipynb
```

## Maintenance notes

### Isolation using Conda

```
conda create --name synimg python=3.6
conda activate synimg
pip install -r requirements.txt
jupyter notebook src/notebook.ipynb
conda deactivate
```

### In progress: Docker usage

Not fully tested, missing `kaggle` dependency but otherwise might be OK.

```
docker run \
-p 8888:8888 \
-v $PWD:/home/jovyan/work \
jupyter/tensorflow-notebook \
jupyter notebook work/src/notebook.ipynb
```

## Background

Machine learning can be used to classify images. It can tell us: "This is a picture of a dog",
"Picasso made this painting", that sort of thing.

### Challenge

I have prepared a collection of computer generated images in different styles (the styles are named
after cities). A bunch of the images have labels indicating their style. Some of them are unlabelled.
We'd like you to figure out the correct labels for the unlabelled images.

The data, and more details, can be found at: <https://www.kaggle.com/c/synthetic-image-classification/>.

That link goes to a Kaggle InClass competition I created. Kaggle is a website for machine learning
competitions. The InClass competitions are academic competitions that don't affect your ranking.

### Submission

What to submit?

* Upload a CSV of image ids and labels to the Kaggle competition.
* You'll need to get me a copy of your code within 48 hours of the Kaggle competition ending, so we can judge it.

When to submit?

* Kaggle competition finishes: 23:59:59 on Thursday July 31st UTC (that's 2 weeks away, people).
* Code to Tim by: 23:59:59 August 2nd UTC

### Criteria for Awesomeness

* Clean Code
* Evidence of TDD
* Score better than the benchmark on the competition leaderboard
* A go script and README (for people submitting solutions to be run locally)
* (Bonus) Evidence of data exploration (you can attach a pdf of a notebook, if you like)
* (Bonus) Analysis of how your algorithm works (activation maps, etc.)
