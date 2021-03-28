# IBM AI Enterprise Workflow Capstone - Alain Buyze

### Are there unit tests for the API?
The unittests are available in the directory **unittests**, the python module **ApiTests.py**
#### First start the FLASK API
Set the current directory to the root of the local replica of the repository
Run the command **python app.py**
Check if the app is runnin by opening **http://0.0.0.0:8080/** - you should seee the welcome page
#### Run the tests

From the root directory of the repository, run **python unittests/piTests.py**
This will execute 4 test:
1. test the train functionality
2. test for appropriate failure in case of no data or ill-formed input
3. test the predict functionality
4. test the log functionality

## Are there unit tests for the model?
The unittests are available in the directory **unittests**, the python module **ModelTests.py**
From the root directory of the repository, run **python unittests/ModelTests.py**
This will execute 3 test:
1. Test the train functionality
2. test if models have been loaded
3. test the predict functionality

## Are there unit tests for the logging?
The unittests are available in the directory **unittests**, the python module **LoggerTests.py**
From the root directory of the repository, run **python unittests/LoggerTests.py**
This will execute 4 test:
1. Test if training log file is created
2. Test if content of Training log file can be retrieved 
3. Test if predict log file is created
4. Test if content of Preduct log file can be retrieved

## Can all of the unit tests be run with a single script and do all of the unit tests pass?
From the root directory of the repository, run **python runtests.py** 
 
## Is there a mechanism to monitor performance?


## Was there an attempt to isolate the read/write unit tests from production models and logs?
This is achieved by the **parameter test=True** in calling the module **update_train_log** and **update_predict_log** in the **LoggerTests.py** module. 
This will ensure that the logfiles names have no date identifier in their name, unlike the regular log files. 


## Does the API work as expected? For example, can you get predictions for a specific country as well as for all countries combined?


## Does the data ingestion exists as a function or script to facilitate automation?


## Were multiple models compared?


## Did the EDA investigation use visualizations?
Check out the Python Notebook **Capstone EDA.ipynb** to see the visualisations used
1. -> graphically the views per month
2. -> revenue per month
3. -> evolution of the Revenue
4. -> view spectral relationship between revenue and date 

## Is everything containerized within a working Docker image?


## Did they use a visualization to compare their model to the baseline model?
