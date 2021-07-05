# Data-Scientist-Capstone-Project
Data Scientist Nanodegree
## Starbucks Capstone Challenge



## Table of Contents

[Introduction](#introduction)

[Problem Statement](#problem-statement)

[Project Motivation](#project-motivation)

[File Descriptions](#file-descriptions)

[Results](#results)

## Introduction
This data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. In this project, I will understand the data and try to provide a solution for how Starbucks should deal with customers, which promotions should provide and to whom? instead of providing offers for all customer which that make the customers who completed offers feel better and may push them to be customers for a long time.<br>
I will combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.<br>

## Problem Statement
The problem is Starbucks give each customer an offer, but there are some customers didn’t use the offer or didn’t view the offer and that is the problem. So I would like to make an analysis of Starbucks datasets to find which kind of people or their demography have an offer and they completed the offer. This segment of people should give them attention and send to them offers. Also, I would like to find which kind of offer (BOGO or Discount or Informational) do people more like or use more. The solution will reduce the overhead cost of sending offers to any customer. For that, I will accuracy metric to evaluate some supervised learning models.<br>

## Project Motivation
In this project, I will analysis the datasets provided by answering these questions  which help to make a decision to solve the problem with visualizations and modeling the dataset:<br>
* Q1: What is the distribution of gender?<br>
* Q2: What is the distribution of income by gender?<br>
* Q3: What are the most and the least common event?<br>
* Q4: What are the most and the least common offer type?<br>
* Q5: What are the most and the least common offer type by offer completed?<br>
* Q6: What is the distribution of gender by offer type?<br>
* Q7: What is the distribution of gender by event?<br>

Then, I will calculate the accuracy metrics for some of the models on the training and testing datasets and improve the best one. I selected accuracy due to the target variable classes in the data and I want to find out the ratio of the total number of predictions that were correct.<br>

## File Descriptions
The data is contained in three files:<br>

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)<br>
  * id (string) - offer id <br>
  * offer_type (string) - type of offer ie BOGO, discount, informational<br>
  * difficulty (int) - minimum required spend to complete an offer<br>
  * reward (int) - reward given for completing an offer<br>
  * duration (int) - time for offer to be open, in days<br>
  * channels (list of strings)<br>
* profile.json - demographic data for each customer<br>
  * age (int) - age of the customer<br>
  * became_member_on (int) - date when customer created an app account<br>
  * gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)<br>
  * id (str) - customer id<br>
  * income (float) - customer's income<br>
* transcript.json - records for transactions, offers received, offers viewed, and offers completed<br>
  * event (str) - record description (ie transaction, offer received, offer viewed, etc.)<br>
  * person (str) - customer id<br>
  * time (int) - time in hours since start of test. The data begins at time t=0<br>
  * value - (dict of strings) - either an offer id or transaction amount depending on the record<br>
  
## Results
Based on the analysis above, there is a 13% difference between male and female who completed the offer of received offer and the females is higher than males. In addition, the favorite offer type for female (43.34%) and male (42.58%) is BOGO then Discount. So, I recommend Starbucks to provide offers for female due to the females’ income mean are 71306 and more than males which are 61194. Even though males purchaser are more than females and the Proportion of transaction for males (87.81%) is higher than females (77.5%). Finally, I think may this decision will change if we have completed dataset and without have missing values.<br>

The main findings of the code can be found at the post available [here](https://yagiz-dursun.medium.com/assessing-starbucks-app-data-c1b0955d03d9).

