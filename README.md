# Short Term Electricity Price Forecasting

This repo provides a sample code that analyses market data from [Nord Pool Electricity Market](https://www.nordpoolgroup.com/) and develop a Machine Learning model for price forecasting. 

The aim of the work is to understand the feasibility of Long Short Term Memory Neural Networks for Time Series Forecasting when dealing with electricity market analysis. This is a state-of-the-art algorithm, compared to classic ARIMA approach, that may lead to important benefits in terms of forecast performance.

## Getting Started

### Prerequisites
1. **Python 3.5** or higher
2. **Python libraries**: numpy, pandas, scipy, matplotlib, keras, tensorflow 


### Clone this repo
```
git clone https://github.com/shreya12-hash/Capstone-project-dsdn.git
```

### Download the dataset

You have two possibilities:

1. Download the original dataset from the historical data download page: [Market Data by Nord Pool](https://www.nordpoolgroup.com/historical-market-data/). You can select any dataset you want. This analysis is performaned using huorly market price data from 2013 to 2018.

2. Use the data already contained in the repository (**data** folder). I have already cleaned some stuff and converted each file into a CSV. The notebooks are supposed to work out-of-the-box with the CSV files I made. 

### Launch Jupyter Notebook

Launch Jupyter from your Anaconda terminal (or any UNIX command line after loading your Python environment):

```
jupyter-notebook
```
Open the notebooks **BASELINE.ipynb** and **LSTM.ipynb** contained in the repo. Run them cell by cell to understand what is going on. Markdown and comments will help you understand each line of code. Each Jupyter containes mostly functions, so that the code is modular and re-usable, easily convertible in class objects for a more efficient .py software.

The content of each notebook is breifly explained:
1. **BASELINE** notebook. A simple persistence model is set as a benchmark for predicting huorly electricity price.
2. **LSTM** notebook. An advanced LSTM model is developed using Keras library. Its performance are assessed with different forecast time horizons. A comparison with baseline allows to understand the benefits of the model. 


## Built With

* [Python](https://www.python.org/) - Python programming language
* [Jupyter](http://www.dropwizard.io/1.0.2/docs/) - iPython Notebook
* [PyCharm](https://www.jetbrains.com/pycharm/) - Python IDE by JetBrains
* [Brackets](https://maven.apache.org/) - My favourite text editor


## Authors

* **Shreya Biswas** - [My GitHub](https://github.com/shreya12-hash)

## License

* This project is licensed under the GPL v3 License - see the **LICENSE.txt** file for details

## Acknowledgments

* Acknowledgement is given to [Nord Pool](https://www.nordpoolgroup.com/) for providing such an extensive and uncommonly clean dataset

## Documentation
* [YouTube lesson](https://www.youtube.com/watch?v=WCUNPb-5EYI) A simple LSTM practical explanation
* [MachineLearningMastery.com](https://machinelearningmastery.com/time-series-forecasting-long-short-term-memory-network-python/) A wonderful website containing many sample codes to learn LSTM applied to different scenarios
