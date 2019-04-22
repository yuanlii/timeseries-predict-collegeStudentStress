# Predict College Student Stress

This project we are interested in exploring college student stress patterns, and develop a stress level prediction system that allows schools and parents to take action to prevent students get stressed out. In order to achieve such goal, we first implemented Granger Causality Analysis to analyze the interrelationships between students' stress level and other factors, including sleeping hours, quality, time spent on exercise, social activities, etc. Then we used three different methods -- Autoregressive (AR) Model, Moving Average(MA) model and an integrated approach (ARIMA) model to predict the overall student stress level within a specific time range.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

pandas
numpy
matplotlib
seaborn
glob
warnings
statsmodels

```
$ pip install statsmodels
```

### Source Data
This project is based on StudentLife & Longitudinal Student Data collected by Dartmouth research center, data can be downloaded from [site](http://studentlife.cs.dartmouth.edu/dataset.html). It contains sensor data, EMA data, survey responses and educational data as well as other scales of students' activities. For this project, We mainly focus on EMA Data, Sensor Data and survey responsed.

### Code Explanation
* AC(log)_vol2.ipynb - implement autocorrelation for time-series modeling, with student stress level log-transformed 
* GC(merged_data).ipynb - implement Granger Causality analysis on student stress level and other daily factors
* baseline_evaluation.ipynb - baseline evaluation
* combine_student_data.ipynb - data preprocessing for combing student data 

### Conclusion
* Detailed report can be downloaded from [here](https://github.com/yuanlii/college_student_stress_prediction/blob/master/project_report.pdf) 
* project poster can be seen [here](https://github.com/yuanlii/college_student_stress_prediction/blob/master/project_poster.pdf)


## Collaborators

* **Yuan Li ** - [github](https://github.com/yuanlii)
* **Crystal Wang ** - [github](https://github.com/Crystalwang0124)


## Acknowledgments
Codes and tutorials below also contribute to this project.

* [时间序列预测全攻略](https://my.oschina.net/zhiyonghe/blog/906307):referenced for implementation of Dickey-Fuller test and time-series modeling
* [手把手教你用 Python 实现针对时间序列预测的特征选择](https://cloud.tencent.com/developer/article/1077714) referenced for autocorrelation plot
