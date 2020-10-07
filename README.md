# Analyze time series data

Analyze and test your time series data using Jupyter Notebook tutorials (.ipynb files) and corresponding sample data (.csv files). We include tutorials and sample data for the following topics:

- [How to generate time series data](/notebooks/Generate_Time_Series.ipynb)
- [How to get started with InfluxDB and Python](/notebooks/Getting_Started_with_InfluxDB_and_Python.ipynb)

- Anomaly detection:
  - For [multiple time series](/tree/Anomaly_Detection/Multiple%20time%20series), including BIRCH, KMEANS, and MAD.
  - For [single time series](/tree/Anomaly_Detection/Single%20time%20series), including Autoregression, LevelShiftAD, and SeasonalAD

- [Forecasting](/tree/Forecasting), including FBProphet and LSTM
 
## Use this repo

Installations of Python can get a bit tricky; different versions of the language, as well as projects which require different versions of installed libraries, can quickly lead to conflicts. Using a virtual environment is reccommended. Please consider looking into additional tooling like [virtualenv](https://pypi.python.org/pypi/virtualenv) or [pyenv](https://github.com/pyenv/pyenv) might be useful.

Run `pip install requirements.txt` inside your virtual environment to download all of the necessary dependencies. 

## Run Jupyter Notebook 
After cloning this repo, [run Jupyter Notebook](https://jupyter.readthedocs.io/en/latest/running.html) locally with `jupyter notebook`. This should direct you to the web application which by default runs on http://localhost:8888. 