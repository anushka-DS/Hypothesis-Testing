# Introduction to Statistics

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/rouseguy/intro2stats/trend.png)](https://bitdeli.com/free "Bitdeli Badge")


Inspired by Allen Downey's books [Think Stats](http://greenteapress.com/thinkstats/) and [Think Bayes](http://greenteapress.com/thinkbayes/), this is an attempt to learn Statistics using an application-centric programming approach. 

## Objective
Showcase real-life examples and what statistics to use in each of those examples. Almost every book teaches a concept and shows an example. Ultimately, every topic gets treated separately and no holistic view is presented. Here, we would take examples and see how to make sense out of it. 

## Topics covered

* Mean, Median, Mode
* Standard Deviation
* Variance
* Co-variance
* Probability Distribution
* Hypothesis Testing
* t-test, p-value, chi-squared test
* Confidence Intervals
* Confidence levels and Sigificance levels
* Correlation
* Resampling (and uses in Big Data)
* A/B Testing
* A simple linear regression model

## Workshop Plan
We would be using Marijuana prices in various states of the USA, along with demographic data of the USA based on the latest census data

There will be separate ipython notebooks - grouped by topic similarities. *notebooks will be uploaded later*
Some examples include:
* Find sum of people buying weed in a year, by various states.
* Find mean of price in a week/month, by various states.
* Find variance of price in selected states. Find variance of selected states by week of month
* Define distribution. Plot histograms
* Determining outliers (Plots, quantiles, box plots, percentiles) in weed price data
* Continuous distributions(exponential distribution, normal distribution)
* Introduction to Probability
* Hypothesis testing. Check if weed price across states are similar or not. Check for different qualities of weed
* Resampling
* Simple regression model: Predict weed price for the next month. Understand the output and diagnostics
* Introduction to A/B testing: Impact of regulation and deregulation on a couple of states 


## Prerequisites
* Basics of Python. User should know how to write functions; read in a text file(csv, txt, fwf) and parse them; conditional and looping constructs; using standard libraries like os, sys; lists, list comprehension, dictionaries
* It is good to know basics of the following:
    * Numpy
    * Scipy
    * Pandas
    * Matplotlib
    * Seaborn
    * IPython and IPython notebook - Everything here would be an IPython notebook
* Software Requirements
    * Python 2.7
    * git - so that this repo can be cloned :)  
    * virtualenv
    * Libraries from *requirements.txt*

## Optional
Users could choose to install Anaconda, if they want. If using Anaconda or Enthought, please ensure that all libraries listed in the requirements.txt are installed. 

*Note to Windows Users*: Neither of us use Windows. From past workshop experiences, Windows users have faced issues installing the way explained below. It is advisable to install Anaconda and ensure that all the libraries listed in the *requirements.txt* file are installed.  

## Setup Guide

#### Clone the repository
    $ git clone https://github.com/rouseguy/intro2stats.git

#### Create a virtual environment & activate
    $ cd intro2stats
    $ virtualenv env
    $ source env/bin/activate

#### Install reqirements from requirements file
    $ pip install -r requirements.txt

#### Note: Make sure you have libraries for png & freetype.
Ubuntu users can install the below

    apt-get install libfreetype6-dev
    apt-get install libpng-dev

### Script to check if installation is fine for the workshop
Please execute the following at the command prompt

    $ python check_env.py

If any library has a `FAIL` message, please install/upgrade that library.

---

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Introduction to Statistics using Python</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://twitter.com/bargava/" property="cc:attributionName" rel="cc:attributionURL">Bargava</a> and <a xmlns:cc="http://creativecommons.org/ns#" href="https://twitter.com/raghothams/" property="cc:attributionName" rel="cc:attributionURL">Raghotham</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.






# Hypothesis-Testing

Hypothesis testing is used to confirm your conclusion (or hypothesis) about the population parameter (which you know from EDA or your intuition). Through hypothesis testing, we can determine whether there is enough evidence to conclude if the hypothesis about the population parameter is true or not.

When evaluating a hypothesis, we need to account for both the variability in your sample and how large your sample is. 


Hypothesis testing is an essential procedure in statistics. A hypothesis test evaluates two mutually exclusive statements about a population to determine which statement is best supported by the sample data. When we say that a finding is statistically significant, it's thanks to a hypothesis test.


**What are the six steps of hypothesis testing?**


**Step 1:** Specify the Null Hypothesis. 

**Step 2:** Specify the Alternative Hypothesis.

**Step 3:** Set the Significance Level 

**Step 4:** Calculate the Test Statistic and Corresponding P-Value.

**Step 5:** Drawing a Conclusion.


**THE ROLE OF HYPOTHESIS TESTS**

We’ve placed our sample mean in the context of all possible sample means while assuming that the null hypothesis is true. Are these results statistically significant?

As you can see, there is no magic place on the distribution curve to make this determination. Instead, we have a continual decrease in the probability of obtaining sample means that are further from the null hypothesis value. Where do we draw the line?

This is where hypothesis tests are useful. A hypothesis test allows us quantify the probability that our sample mean is unusual.

For this series of posts, I’ll continue to use this graphical framework and add in the significance level, P value, and confidence interval to show how hypothesis tests work and what statistical significance really means.


**Part Two:** Significance Levels (alpha) and P values  (https://blog.minitab.com/en/adventures-in-statistics-2/understanding-hypothesis-tests-significance-levels-alpha-and-p-values-in-statistics)

**Part Three:** Confidence Intervals and Confidence Levels  (https://blog.minitab.com/en/adventures-in-statistics-2/understanding-hypothesis-tests-confidence-intervals-and-confidence-levels)


**Important links :**

https://machinelearningmastery.com/statistical-hypothesis-tests/
https://online.stat.psu.edu/stat502/lesson/1/1.2
https://www.optimizely.com/optimization-glossary/ab-testing/
https://www.tutorialspoint.com/statistics/hypothesis_testing.htm
https://www.statisticshowto.com/probability-and-statistics/hypothesis-testing/
https://www.analyticsvidhya.com/blog/2015/09/hypothesis-testing-explained/
https://analyticsindiamag.com/importance-of-hypothesis-testing-in-data-science/
https://medium.com/ml-ai-study-group/confidence-interval-confidence-level-be58d250dd40#
https://www.nedarc.org/statisticalhelp/advancedstatisticaltopics/hypothesisTesting.html
https://analyticsindiamag.com/10-most-popular-statistical-hypothesis-testing-methods-using-python/


**A/B Test**
https://www.optimizely.com/optimization-glossary/ab-testing/

**Chi-Square test**
https://www.statisticshowto.com/probability-and-statistics/chi-square/

**ANOVA**  https://www.statisticshowto.com/probability-and-statistics/hypothesis-testing/anova/


