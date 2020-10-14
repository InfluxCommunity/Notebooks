# Analyze time series data and experiment with ML Algorithms

Jupyter Notebooks are wonderful because they provide a way to share code, explanations, and visualizations in the same place. Notebooks add narrative to computation. The cells compartmentalize steps and fascilitate data analysis. In this way, notebooks act as an invitation for experimentation. If you are looking to enhance your time series data by performing time series data analytics or data science tasks, a Notebook is a great place to start this work. 

Analyze your time series data and experiment with forecasting and anomaly detection algorithms using Jupyter Notebook tutorials (.ipynb files) and corresponding sample data (.csv files). We include tutorials and sample data for the following topics:

- [How to generate time series data](Generate_Time_Series.ipynb)
- [How to get started with InfluxDB and Python](Getting_Started_with_InfluxDB_and_Python.ipynb)
- [How to get started with InfluxDB and Pandas](Getting_Started_with_InfluxDB_and_Pandas.ipynb)
- [How to get started with Jupyter and Flux](Getting_Started_with_Jupyter_and_Flux.ipynb)

- [Anomaly detection](/Anomaly_Detection):
  - For [multiple time series](/Anomaly_Detection/Multiple_time_series), including BIRCH, KMEANS, and Median Absolute Deviation(MAD).
  - For [single time series](/Anomaly_Detection/Single_time_series), including Autoregression, LevelShiftAD, and SeasonalAD

- [Forecasting](/Forecasting), including [FBProphet](https://facebook.github.io/prophet/) and LSTM with [Keras](https://keras.io/)
 

## Set up this repo

These instructions are written for InfluxDB OSS 2.0 release candidate 0 and later or InfluxDB Cloud. If you're using InfluxDB Cloud make sure to change your URL appropriately.  

Installations of Python can get a bit tricky; different versions of the language, as well as projects which require different versions of installed libraries, can quickly lead to conflicts. Using a virtual environment is reccommended. Please consider looking into additional tooling like [virtualenv](https://pypi.python.org/pypi/virtualenv) or [pyenv](https://github.com/pyenv/pyenv) might be useful.

Run `pip install requirements.txt` inside your virtual environment to download all of the necessary dependencies. 

After cloning this repo, [run Jupyter Notebook](https://jupyter.readthedocs.io/en/latest/running.html) locally with `jupyter notebook`. This should direct you to the web application which by default runs on http://localhost:8888. 


## Implementation Options and Recommendations 

After you analyze your time series data with notebooks and select the forecasting or anomaly detection approach that works for you, it's time to implement your solution in production. The following resources could be useful in that next step: 
- Using the [http.post()](https://docs.influxdata.com/influxdb/v2.0/reference/flux/stdlib/http/post/) function in a [task](https://docs.influxdata.com/influxdb/v2.0/process-data/manage-tasks/) in combination with a serverless compute solution (like [aws lambda](https://aws.amazon.com/lambda/) for example) to run your code. 
- Using the [Telegraf Execd processor plugin](https://github.com/influxdata/telegraf/tree/master/plugins/processors/execd) to run an external program. Please see this example of [Machine Learning with the Telegraf Execd processor plugin](https://github.com/influxdata/tg-brew-anomaly) for more details. 

## Additional Resources 

This repo is just a sample of some of the many algorithms, approaches, and tools to time series forecasting and anomaly detection. Here are additional ML solutions that might interest the reader:

- [STUMPY](https://github.com/TDAmeritrade/stumpy): "A powerful library that efficiently computes the [matrix profile](https://stumpy.readthedocs.io/en/latest/Tutorial_The_Matrix_Profile.html) of a time series, which can be used for a variety of time series data mining tasks.
- [scikit-multiflow](https://scikit-multiflow.github.io/): A machine learning package for streaming data in Python, especially apt for clustering. 
- [InfluxDB Interpreter for Apache Zeppelin](https://github.com/apache/zeppelin/tree/master/influxdb): Apache Zeppelin is another web-based notebook similar to Jupyter Notebooks. Zeppelin has built in [Spark](https://spark.apache.org/) integration. Zeppelin and the InfluxDB interpreter enables easy access to and parallelization of big time series data for quick analysis on large volumes of data. 