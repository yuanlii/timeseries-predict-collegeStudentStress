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
This project is based on data from  ...

The data set we will dive into is the students activities monitor data and the mental health survey results. The whole data set includes several aspects information, for example, the sensor data which record the daily activities of the students,
and the survey results which indicate the mental health status of the students. The system will combine the two types of data and find the connection between physical activities and mental health status.

StudentLife Dataset contains the sensor data, EMA data, survey responses and educational data. We would mainly focus on the data about students’ behavior and activities of how they interact with the world, for example, measurements of activities, behavior, events, exercise (from the EMA Data), and other measurements of activities, audio,conversation, etc. (from Sensor Data) would be interesting for further exploration.

### Code Explanation
* AC(log)_vol2.ipynb - implement autocorrelation for time-series modeling, with student stress level log-transformed 
* GC(merged_data).ipynb - implement Granger Causality analysis on student stress level and other daily factors
* baseline_evaluation.ipynb - baseline evaluation
* combine_student_data.ipynb - data preprocessing for combing student data 

### Conclusion
* TODO
* Detailed report


## Collaborators

* **Yuan Li ** - [github](https://github.com/yuanlii)
* **Crystal Wang ** - [PurpleBooth](https://github.com/PurpleBooth)


## Acknowledgments
Codes and tutorials below also contribute to this project.

* [时间序列预测全攻略](https://my.oschina.net/zhiyonghe/blog/906307):referenced for implementation of Dickey-Fuller test and time-series modeling
* [手把手教你用 Python 实现针对时间序列预测的特征选择](https://cloud.tencent.com/developer/article/1077714) referenced for autocorrelation plot
