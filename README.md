# Instacart Reorder Prediction & Market Basket Analysis

> An exploratory data analytics study that walks through a practical, end-to-end workflow on a InstaCart Market Basket dataset. It demonstrates how to prepare messy data with clear cleaning steps, compute useful statistical summaries to understand distributions and trends, and create visualizations that make patterns easy to interpret. The goal of this project was to find a solution to the PROBLEM STATEMENT through the exploration of these RESEARCH QUESTIONS or OBJECTIVES.

---

## Overview

This project was completed for the SDC486L Data Analytics course.  
It applies exploratory data analysis, classification modeling, neural networks, and market basket analysis to understand customer reorder behavior and generate actionable business insights.

---

## Objectives

- Predict whether a product will be reordered  
- Identify products frequently purchased together  
- Analyze how order timing impacts reorder probability  
- Simulate real-world scenarios using a trained neural network  

---

## Dataset

**Source:** Instacart Online Grocery Basket Analysis Dataset (Kaggle)

- ~1.05 million grocery orders  
- Order timing data (day, hour, days since prior order)  
- Product and department information  
- Binary target variable: `reordered`  

---

## Modeling Approach

### Baseline Model – Logistic Regression
- Accuracy: 0.67  
- F1-Score: 0.75  

### Neural Network
- Two hidden layers (64, 32 neurons)
- ReLU activations, Sigmoid output
- Accuracy: 0.68  
- F1-Score: 0.75  

The neural network slightly improved overall performance.

---

## Market Basket Analysis

Product associations were analyzed using Lift.  
A heatmap visualization highlights strong product pair relationships that support recommendation strategies.

---

## Scenario Analysis

Three timing scenarios were simulated:

- Weekend orders  
- Evening orders  
- Long purchase gap (30 days)  

**Key Finding:**  
Recency (days since prior order) significantly reduces reorder probability, while day-of-week and hour-of-day have minimal impact.

---

## Key Insights

- ~60% of items are reordered  
- Recency is the strongest predictor of reorder behavior  
- Neural networks slightly outperform Logistic Regression  
- Product associations support cross-selling strategies  

---

## Dashboard

An interactive Power BI dashboard includes:

- Model performance comparison  
- Reorder trends by timing  
- Lift heatmap of product associations  
- Scenario impact comparison  

---

## Project Presentation Video

Project Presentation Video:  
https://youtu.be/fOJ4Lxh8rlY

---

## Author

John Proctor
SDC486L – Data Analytics
