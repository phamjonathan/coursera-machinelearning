### Intro to Machine Learning

Machine Learning (new computer capability) “Computer Systems People”
to apply learning algorithms to their own problems.
* Grew out of work in AI
* New capability for computers

#### Examples:

* Database mining
    * Large datasets from growth of automation/web.
    * E.g., Web click data, medical records, biology, engineering.
* Applications can’t be programmed by hand.
    * E.g., Autonomous helicopter, handwriting recognition, most of Natural Language Processing (NLP), Computer Vision.
* Self-customizing programs 
    * E.g., Amazon, Netflix product recommendations
* Understanding human learning (brain, real AI)

#### Machine Learning Definition

`Arthur Samuel (1959)` Machine Learning: Field of study that gives computers the ability to learn without being explicitly programmed.

`Tom Mitchell (1998)` Well-posed Learning Problem: A computer program is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T, as measured by P, improves with experience E.

Suppose your email program watches which emails you do or do not mark as spam, and based on that learns how to better filter spam. What is the task T in this setting?

A) Classifying emails as spam or not spam (T)

B) Watching you label emails as spam or not spam. (E)

C) The number (or fraction) of emails correctly classified as spam/not spam. (P)

D) None of the above— this is not a machine learning problem. 

#### Two Broad Classifications:

`Supervised Learning`

In supervised learning, we are given a data set and already know what our correct output should look like, having the idea that there is a relationship between the input and the output.
Supervised learning problems are categorized into "regression" and "classification" problems. In a regression problem, we are trying to predict results within a continuous output, meaning that we are trying to map input variables to some continuous function. In a classification problem, we are instead trying to predict results in a discrete output. In other words, we are trying to map input variables into discrete categories.

Example 1:

Given data about the size of houses on the real estate market, try to predict their price. Price as a function of size is a continuous output, so this is a regression problem. We could turn this example into a classification problem by instead making our output about whether the house "sells for more or less than the asking price." Here we are classifying the houses based on price into two discrete categories.

Example 2:

(a) `Regression` - Given a picture of a person, we have to predict their age on the basis of the given picture

(b) `Classification` - Given a patient with a tumor, we have to predict whether the tumor is malignant or benign.

`Unsupervised Learning`

Unsupervised learning allows us to approach problems with little or no idea what our results should look like. We can derive structure from data where we don't necessarily know the effect of the variables. We can derive this structure by clustering the data based on relationships among the variables in the data.
With unsupervised learning there is no feedback based on the prediction results.

Example:
Clustering: Take a collection of 1,000,000 different genes, and find a way to automatically group these genes into groups that are somehow similar or related by different variables, such as lifespan, location, roles, and so on.
Non-clustering: The "Cocktail Party Algorithm", allows you to find structure in a chaotic environment. (i.e. identifying individual voices and music from a mesh of sounds at a cocktail party).

