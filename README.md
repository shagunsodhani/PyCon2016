# PyCon2016
Code and Presentation for PyCon2016

## Topic

[Big Data Analysis using PySpark](https://in.pycon.org/cfp/2016/proposals/big-data-analysis-using-pyspark~b8Mld/)

## Presentation

* [Introductory Slides](https://slides.com/shagunsodhani/pycon2016)
* [Exploratory Analysis Demo](http://shagunsodhani.in/PyCon2016/presentation/StackOverflow/User/ExploratoryAnalysis.slides.html)
* [Word2Vec Demo](http://shagunsodhani.in/PyCon2016/presentation/AskUbuntu/Question/Word2Vec.slides.html)

## Local Setup

* Follow the instructions on [iota](https://github.com/shagunsodhani/iota) to setup execution environment and get and process the raw StackExchange Data.
* `cd notebook`
* `./run.sh`

## Databricks Community Edition

* [Sign up for free community version edition of Databricks](https://databricks.com/try-databricks)
* Create a new spark cluster (Spark 1.6.1 and Hadoop 2)
* To import the Jupyter Notebooks from `notebook` directory, select **Workspace** option from the menu in the left, click on the dropdown next to the username and select **Import**.
![alt tag](https://d37djvu3ytnwxt.cloudfront.net/assets/courseware/v1/b24280c52ad86033de804a6e1ce17fd6/asset-v1:BerkeleyX+CS105x+1T2016+type@asset+block/Import1.png)
* Select the URL option, paste the url of the notebook and click **Import**. For example, url of Word2Vec notebook is  https://github.com/shagunsodhani/PyCon2016/blob/master/notebook/AskUbuntu/Question/Word2Vec.ipynb
* Fetch the processed parquet files from [here](https://dl.dropboxusercontent.com/u/56860240/PyCon2016/data.zip), upload them to Databricks as explained [here](https://docs.cloud.databricks.com/docs/latest/databricks_guide/03%20Data%20Sources/1%20Data%20Import%20UI.html) and set the `use_local_datapath` to `False` and `dbfs_user_data_path` and `dbfs_question_data_path` to path where parquet files are uploaded.

## Dataset

* Processed data (which is used for demo) can be downloaded [here](https://dl.dropboxusercontent.com/u/56860240/PyCon2016/data.zip).
* For getting the latest version of data, follow the instructions on [iota](https://github.com/shagunsodhani/iota) to setup execution environment and get and process the raw StackExchange Data.

## More Notebooks

* This repo only contains notebooks which will be demoed at PyCon2016.
* For more notebooks related to Stack Exchange data, check out [iota](https://github.com/shagunsodhani/iota)

## Attribution

The [image](https://d37djvu3ytnwxt.cloudfront.net/assets/courseware/v1/b24280c52ad86033de804a6e1ce17fd6/asset-v1:BerkeleyX+CS105x+1T2016+type@asset+block/Import1.png) showing the workflow to import the notebooks is created by [Databricks](https://databricks.com). Licence at [https://creativecommons.org/licenses/by-nc-nd/4.0/](https://creativecommons.org/licenses/by-nc-nd/4.0/)