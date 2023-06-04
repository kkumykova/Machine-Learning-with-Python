# Machine Learning with Python

**[Introduction to machine learning course](https://www.thegreatcourses.com/courses/introduction-to-machine-learning)**

**[Great courses - Machine Learning](https://github.com/mlittmancs/great_courses_ml)**

**[Great courses - Colab](https://colab.research.google.com/github/mlittmancs/great_courses_ml/blob/master/)**

---



![ml](https://i.imgur.com/dPoSllF.png)

**ML = desires output + data to desire rules.**

- A computer uses data to write its own program.
- We help the computer just enough to help find the rules.
- We don't tell the computer the rules explicitly.

**There are five main schools of ML:**
1. Decision Trees (reasoning with symbols)
2. Neural Networks incl. perceptron, deep networks (analyzing perceptual information)
3. Bayesian Networks (managing uncertainty)
4. Genetic programs (discovering new structures)
5. Nearest neighbours (exploiting similarities)
The five can and should work together.
Decision trees are used for medical diagnosis.
Deep networks have three layers.
Bayesian Networks assign probabilities to diagnosis.

**Find a way to evaluate the rule.**

We need a scoring function - **a loss function** - calculates how accurate the rules is based on the data.
Scores can be used indirectly to define the rule.

---

## Three components of ML
1. represent - representational space
2. evaluate - loss function on data
3. select - optimiser
Optimiser selects the rule with the best available score from the representational space.
Some loss functions penalise a rule based on its complexity.
Loss functions assigning the scores to evaluate each candidate's rules.
What ML does is to approximately optimise loss over the representational space.

---

## Basic recipe for ML program:
1. choose a representational space
2. design a loss function that uses data to score potential rules
3. run an optimiser that selects the rule in the representational space with the approximately best score.
---

**ML turns data into rules.**

Basic recipe for a ML program:

1. choose a representational space

2. design a loss function that uses data to score potential rules

3. run an optimiser that selects the rule in the representational space with the approximately best score.

ML turns data into rules.

Example for ML program components for a driving route:

| Component | Example |
|------|-------|
| Rule | route |
|Representational space|all possible routes|
|Loss function on data|estimated time of a route|

---

Traditional programming - imperative programming (tell the computer what to do).

ML - declarative programming (tell the computer what to “like).

---

## ML Types

1. Supervised learning (input and output or labels are provided)

2. Unsupervised learning 

3. Semi-supervised learning (some examples are given to shed light on the rest)

4. Reinforcement learning (something between supervised and unsupervised learning): labels are evaluations indicating how good the given answer is. The program does not tell you the exact “right” answer but is giving you the feedback on how well you did it. It’s best used when it is easy to select who wins but the strategy to it is not easy to select.

---
# Decision Trees for Logical Rules
CART: classification and regression trees = decision trees (logical trees with top-down structure)

You cannot do machine learning on data you do not have.

Decision tree is a rule that distinguishes positive and negative examples of a concept.

Binary classification tasks - when you want to separate the input into one of two classes - a prototypical ML problem.

Recursion - applying the same procedure repeatedly to simpler and simpler versions of the same problem.

To build our decision tree top-down we need to answer two big questions:

 Which node to pick first?

Use the average Gini index to calculate the purity score.

When to stop splitting the data and assign a label (try to predict a label)?


## Decision Trees for Logical Rules

![decision trees](https://www.xoriant.com/cdn/ff/weqpbrtpXGjLpVQ_X-gWqsFlvjAxpv5Wv3xNW0A4vuQ/1602007254/public/2020-10/a-decisionTreesforClassification-AMachineLearningAlgorithm.jpg)

**CART**: classification and regression trees = decision trees (logical trees with top-down structure)

* You cannot do machine learning on data you do not have.

* **Decision tree**: a rule that distinguishes positive and negative examples of a concept.

* **Binary classification tasks** - is used when you want to separate the input into one of two classes - a prototypical ML problem.

* **Recursion** - applying the same procedure repeatedly to simpler and simpler versions of the same problem.

* To build our decision tree top-down we need to answer two big questions:

---

 ## Which node to pick first?

**Use the average Gini index to calculate the purity score.**

At wat point should you stop splitting the data and assign a label (try to predict a label)?

---
# Neural Networks for Perceptual Rules 

**Perception**: mapping low-level sensory data to high-level concepts.

**Activation**: number of how excited each unit is.

**Acyclic**: no unit's value can be based, even indirectly, on its own value.

**Activation of a unit**: obtained by taking weighted sum of activations of all units that connect to it.

**Popular activation functions**:
1. linear
2. sigmoid
3. ReLU (rectified linear unit)

**Training a neural network**: a process of finding weight values that result in the desired computation.
