Q1.
**What is the difference between ML (Machine Learning) and AI (Artificial Intelligence)?**

The main difference seems to be quite simple, the idea that ML is programming computers in order to ensure that they can *learn by themselves*, versus AI which is *programming computers such that they are capable of logic and reasoning*

Q2
**Which of the following is the most reasonable definition of machine learning?  
(a) Machine learning is the field of allowing robots to act intelligently.  
(b) Machine learning is the science of programming computers.  
(c) Machine learning only learn from unlabeled data.  
(d) Machine learning is the field of study that gives computers the ability to learn without being explicitly  
programmed.**

1. Deosnt make too much sense as it is not very very clear on what acting intelligently even means. For 2, Machine Learning is not the science of programming computers, if anything this is just *automation*
2. for (C), this is not true as machines can learn from unlabeled (unsupervised learning) and supervised learning
3. This makes the most sense, hence this must be d

Q3
**A computer program is said to learn from experience E with respect to some task T and some performance measure  
P, if its performance on T, as measured by P, improves with experience E. Suppose we feed a learning algorithm a lot  
of historical weather data, and have it learn to predict weather. In this setting what is T?  
(a) The historical weather data.  
(b) The probability of it correctly predicting a future data’s weather.  
(c) The weather prediction task.  
(d) None of these.**

Logically, the answer must be c. The task in this case is the idea of weather prediction

Q4
**Suppose you are working on weather prediction and use a learning algorithm to predict tomorrow’s temperature (in  
degrees Centigrade/Fahrenheit).  
(i) Would you treat this as a classification or a regression problem?  
(a) Regression.  
(b) Classification.  
(c) Clustering.  
(d) None of these.  
(ii) What kind of data should you gather?**

Well, this is a regression problem, as you are trying to find predict the weather tomorrow based on data which was supplied to one before. One could consider this to be a classification problem, but we would first need to understand what kind of datatypes are centigrade and Farehnheit

Q5
**You want to develop learning algorithms to address each of the following two problems.  
P1: You’d like the software to examine your email accounts, and decide whether each email is a spam or not.  
P2: You have a large quantity of green tea (e.g., 1000kg) with a record of previous sales. You want to predict how  
much of it will sell over the next 6 months.  
Should you treat these as classification or as regression problems?  
(a) Treat both P1, P2 Æ regression problems.  
(b) Treat both P1, P2 Æ classification problems.  
(c) Treat P1 Æ regression problem, P2 Æ classification problem.  
(d) Treat P1 Æ classification problem, P2 Æ regression problem.**

P1 is classification
P2 is regression


Q6
**Suppose you are working on stock market prediction. Typically tens of millions of shares of a company’s stock are  
traded each day. You would like to predict the number of shares that will be traded tomorrow.  
(i) Would you treat this as a classification or a regression problem?  
(a) Regression.  
(b) Classification.  
(c) Clustering.  
(d) None of these.  
(ii) If the data you have collected involved millions of attributes, what would you do?**

This can also be considered to be a regression problem


Q7
**Some of the problems below are best addressed using a supervised learning algorithm, and the others with an  
unsupervised learning algorithm. Which of the following would you apply supervised learning to? (Select all that  
apply) Assume some appropriate dataset is available for your algorithm to learn from.  
(a) Determine whether there are vocals (i.e., a human voice singing) in each audio clip extracted from a piece of  
music, or it is a clip of only musical instruments and no vocals.  
(b) Given data on how 1000 medical patients respond to an experimental drug (such as effectiveness of the  
treatment, side effects, etc.), discover whether there are different categories or “types” of patients in terms of  
how they respond to the drug, and if so what these categories are.  
(c) Given a large dataset of medical records of patients suffering from heart disease, try to learn whether there  
might be different clusters of such patients for which we might tailor separate treatments.  
(d) Given a set of data which contains the diet and the occurrence of diabetes from a population over a 10-year  
period. Predict the odds of a person developing diabetes over the next 10 years.**

There are a few things to consider in this question
1. Since we are trying to determoine whether there is human voice or not, we can assume that this data would have to be labeled, as the piece is extracted from some song
2. This is not labelled, hence this must be unsupervised
3. This is not labelled either, hence this is unsupervised
4. regression must have some data to work with, hence this is supervised

Q8.
**Suppose you are working on a machine learning algorithm to predict if a patient is COVID-19 infected according to  
the patient’s particulars such as age and health conditions, symptomatic data, such as fever, dry cough, tiredness,  
aches and pains, sore throat, diarrhoea, conjunctivitis, and headache etc. What are the Task, Performance, and  
Experience involved according to the definition of machine learning?**

- Experience is the Sympotamtic Data and Actual Diagnosis
- Task is patient classification
- The performance measure is the accuracy of the classification


Q9.
**We use labelled data for supervised learning, where the labels are used as the desired target of prediction for  
classifiers. Which of the next data are the useful labelled data?  
(a) To build an image object classifier to discriminate between apple and orange, we have many fruit images  
labelled with the country of origin.  
(b) To build a system to predict the number of COVID cases for tomorrow given the past daily record, we have  
a collection of daily data for a period of 12 months.  
(c) To build a classifier to automatically evaluate student essays, we have collected a set of student essays that  
have not been graded by teachers.**

Only b, as the others are leaving far too much gap from what is expected


Q10.
**Determine whether each of the following is “inductive” or “deductive” reasoning?  
(a) The first coin I pulled from the bag is a penny. The second and the third coins from the bag are also pennies.  
Therefore, all the coins in the bag are pennies.  
(b) All men are mortal. Harold is a man. Therefore, Harold is mortal.**

Both are deductive? But based on the definition, (A) could be inductive as the chance for errors is so high. Also need to know that (a) is built off probable conclusions.

Q11.
