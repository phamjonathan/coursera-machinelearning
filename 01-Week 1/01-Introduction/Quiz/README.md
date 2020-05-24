#### Question 1:

A computer program is said to learn from experience E with 
respect to some task T and some performance measure P if its
performance on T, as measured by P, improves with experience E.
Suppose we feed a learning algorithm a lot of historical weather
data, and have it learn to predict weather. In this setting, what is T?

A) The weather prediction task.

B) The probability of it correctly predicting a future date's weather.

C) The process of the algorithm examining a large amount of historical weather data.

Answer: C 

Explanation: The task described is weather prediction, so this is Task T.

#### Question 2:

Suppose you are working on weather prediction, and you would like to predict whether or not it will be raining at 5pm tomorrow. You want to use a learning algorithm for this. Would you treat this as a classification or a regression problem?

Answer: Classification

Explanation: Classification is appropriate when we are trying to predict one of a small number of discrete-valued outputs, such as whether it is sunny, cloudy, or rainy. 

#### Question 3:

Suppose you are working on stock market prediction, and you would like to predict the price of a particular stock tomorrow (measured in dollars). You want to use a learning algorithm for this. Would you treat this as a classification or a regression problem?

Answer: Regression

Explanation: Regression is appropriate when we are trying to predict a continuous-valued output.

#### Question 4: 

Some of the problems below are best addressed using a supervised learning algorithm, and the others with an unsupervised learning algorithm. Which of the following would you apply supervised learning to? (Select all that apply.) In each case, assume some appropriate dataset is available for your algorithm to learn from.

A) Given a large dataset of medical records from patients suffering from heart disease, try to learn whether there might be different clusters of such patients for which we might tailor separate treatements.

B) Given genetic (DNA) data from a person, predict the odds of him/her developing diabetes over the next 10 years.

C) Examine a large collection of emails that are known to be spam email, to discover if there are sub-types of spam mail.

D) Take a collection of 1000 essays written on the US Economy, and find a way to automatically group these essays into a small number of groups of essays that are somehow "similar" or "related".

Answer: B

Explanation: This can be addressed as a supervised learning, classification, problem, where we can learn from a labeled dataset comprising different people's genetic data, and labels telling us if they had developed diabetes.

#### Question 5:

Which of these is a reasonable definition of machine learning?

A) Machine learning is the field of allowing robots to act intelligently.

B) Machine learning is the field of study that gives computers the ability to learn without being explicitly programmed.

C) Machine learning learns from labeled data.

D) Machine learning is the science of programming computers.

Answer: B

Explanation: This was the definition given by Arthur Samuel.
