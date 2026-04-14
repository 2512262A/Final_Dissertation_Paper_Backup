# Pump-and-Dump Detection using Machine Learning

## Overview
This project develops a machine learning approach to detect pump-and-dump events in financial markets by combining financial and social data. Multiple models are evaluated to determine the most effective approach, and the project also explores predicting when such events are likely to end.

## Motivation
Pump-and-dump schemes manipulate asset prices and mislead investors. Detecting these events early can help reduce financial risk and improve market transparency.

## Features
- Detects pump-and-dump events using machine learning models
- Integrates financial market data and social media signals
- Compares performance across multiple models
- Explores prediction of when pump-and-dump cycles end

## Dataset
This project uses:
- Financial data (OHCLV data of Cryptocurrencies)
- Social data (tweets)

For detailed dataset information, refer to the full paper included in this repository.

## Models
The following models are explored:
- Logistic Regression
- Support Vector Classifier
- Naive Bayes
- Random Forest Classifier

## Results
Models are evaluated using metrics such as accuracy, precision, recall, and F1-score. The best-performing model is identified based on these metrics.

For full evaluation details and analysis, please see the project paper.

## Conclusion
This project developed machine learning models using both market (financial) and social data. Experimental results show that a **Random Forest Classifier using only financial features with a 15-minute window** performed best, achieving:

- **Validation Set**: Precision (0.974), Recall (0.978), F1-score (0.976)  
- **Test Set**: High recall (0.971) but significantly lower precision and F1-score  

Results suggest that **social data did not improve performance**, likely due to lower data density and added noise compared to financial signals.

For predicting the end of pump-and-dump events, the model achieved moderate performance (~65.8% accuracy), but struggled to:
- Accurately detect when a pump ends  
- Avoid early predictions of pump timing  

Overall, the findings highlight that **feature quality and alignment are critical**, and that more robust methods for identifying pump termination are needed to improve prediction performance.

## Paper
The full project report is included in this repository as a PDF for reference.

## Repository

The source code for this project is available on GitLab:  
[View Repository](https://stgit.dcs.gla.ac.uk/2512262a/individual-project)

