# Welcome to the Machine Learning Challenge for SECU0050 and SECU0057.

## Background
In this part of the assessment, you can put your text mining and machine learning skills to use. The machine learning challenge is inspired by so-called "shared tasks" and Kaggle-challenges, where many researchers/analysts compete against each other in solving one problem.

The problem is typically a classification challenge: you are provided with training data that allow you to build a classification system that learns to differentiate between two (or more) outcomes. For example, the training data could consist of movie reviews and a label associated with them (e.g. positive review vs negative review). The task is to build a classification system (i.e. extracting variables needed for classification and choosing algorithms) that you submit and evaluate at a later stage on unseen (i.e. new) data (so-called test data).

## Competition topic
In the machine learning challenge, you will work on a problem from adversarial machine learning. In adversarial machine learning, you have two systems (machine learning-based): for example, one system performs a classification task (e.g. dog vs cat images). The second system (= the adversary) learns how the first system does this and then perturbs (i.e. alters) the input (e.g. cat or dog images) so that the classification system is fooled.

An example is cat images that are perturbed on the individual pixel-level so that an otherwise well-performing classifier confuses it for a dog - while - to the human eye - there is no perceptible change in the image (i.e. we still see it as a cat).

This task has recently been transferred to natural language processing. One setup here is that a classifier tries to discriminate between positive and negative movie reviews, and an adversarial system learns to re-write the reviews so that the classifier mistakes a positive review for a negative one and vice versa. Just as the perturbed image tries to preserve what we see on the image, text-based adversarial perturbations, try to preserve the meaning.

The context of natural language, however, is less forgiving than images: changing a single pixel might not ever be noticed, but an awkward word or strange phrase might be a give-away clue that something is off.

For this challenge, you will work on a dataset of original vs perturbed movie reviews. The task consists of building a classification system that can distinguish between human-written originals and computer-altered adversarial perturbations. The dataset consists of three columns:

column 1: id (the identifier of the datapoint)
column 2: the text data
column 3: the label (original vs perturbed)
Each row represents one data point.
