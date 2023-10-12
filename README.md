# Data Pipeline Project

This repository contains the second project of the neuefische MLE bootcamp.


## Project overview

The aim of this project was to build a data pipeline that is processing the `Green Taxi Trips` of the NYC Taxi Trip Dataset by uploading the data directly into a GCS bucket and then processing it either with a ETL or ELT pipeline to calculate the revenue per day.

### Data upload

The [data_ingestion.py](./src/data_ingestion.py) file in the `src` folder downloads the data for the first three month of the year 2021 from the NY Taxi website and uploads it into a bucket on GCS. 

**Workflow:**
* create service account on google cloud with necessary permissions
* create bucket on google cloud storage
* run [data_ingestion.py](./src/data_ingestion.py) file to get the data from the NY City government page and upload it to the bucket

### Pipeline