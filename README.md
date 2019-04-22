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

### Code Explanation
* AC(log)_vol2.ipynb - implement autocorrelation for time-series modeling, with student stress level log-transformed 
* GC(merged_data).ipynb - implement Granger Causality analysis on student stress level and other daily factors
* baseline_evaluation.ipynb - baseline evaluation
* combine_student_data.ipynb - data preprocessing for combing student data 





### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

