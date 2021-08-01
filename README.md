# Analyze A/B Test Results

An Udacity project regarding the course Data Analyst Nanodegreee.

## Project Overview

This project aims to give you the understanding of the results of an A/B test run by an e-commerce website. The company developed a **new web page** in order to try and increase the number of users who decide to pay for the company's products (this is called **convert**) The goal of the project is to help the company decide whether to keep the old page or implement the new page.

The project takes you through 3 parts:
1. Probability
2. A/B Test
3. Regression testing

The user must go through all of these to explore the data and arrive at meaningful conclusions.


## Results

for every part we got a result on the same dataset:

### Part I: Probability

From using simple probability we can conclude that a user in the **control** group had a **12.04%** chance to convert, whereas a user in the **treatment** group had an **11.88%** chance to convert. From this we may conclude that the control page is better purely due to statistics. However it is a very insignificant difference (0.16%) to decide a certain page will cause more impact.

### Part II: A/B Test

Here we create our hypothesis notation:

**H0: Pnew − Pold ≤ 0**

**H1: Pnew − Pold > 0**

At the end of the section, we calculated the p-value to be 90.62%. Given a large p-value it suggests that we wouldn't move away from the null hypothesis. Also, the p-value is larger than 5% (Type I Error rate).
From that, we **fail to reject the null hypothesis**. Meaning we cannot conclude that the new page converts more users than the old page.

### Part III: Regression

For regression part, we had to use the statsmodel library using the LOGISTIC REGRESSION method. The main difference Part III has on Part II is that in the previous part we did a one-tailed hypothesis test. Whereas in Part III, we do a two-tail test:

Part III Hypothesis:

**H0: Pnew − Pold = 0**
 
**H1: Pnew − Pold ≠ 0**

The p-value that we found above is 0.19. Which means that we also **Fail to reject the null hypothesis** since our Type I error is 0.05 and in order to reject we need to have it less than 0.05.

## Tools

* pandas
* numpy
* random
* matplotlib
* statsmodel



## Statistical Methods and Techniques

* bootstrapping
* Z-test and Critical Z score
* P-value
* Logistic Regression and Dummy Creation
* Hypothesis Testing




