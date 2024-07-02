<div align="center">
  <h1 style="color:#8a2be2;">🚖 Uber Data Analytics | Data Engineering GCP Project☁️</h1>
</div>

## 📖 Introduction
Welcome to the **Uber Data Analytics** project! The goal of this project is to perform data analytics on Uber data using various cutting-edge tools and technologies. 
Here's the project's workflow:

## 🚀 Project Workflow

### 1. Data Ingestion 📥
- **Google Storage**: Raw data is ingested from the TLC Trip Record Data into Google Storage, providing a reliable storage solution for large datasets.

### 2. Data Modeling 🏗️
- **Fact and Dimension Tables**: The data is structured into fact and dimension tables to facilitate efficient querying and analysis.1

### 3. Data Transformation 🔄
- **Python Scripts**: Transformation logic is written in Python to clean, preprocess, and transform the data.
- **Compute Engine**: The transformation code is executed on a Google Compute Engine instance where Mage is installed.

### 4. Data Loading 📤
- **BigQuery**: Transformed data is loaded into BigQuery for scalable and fast querying.

### 5. Data Visualization 📊
- **Looker Studio**: Interactive dashboards are created in Looker Studio to visualize the insights derived from the data.

### Google Cloud Platform ☁️
GCP offers a comprehensive suite of services that are utilized throughout the project to handle storage, computation, data warehousing, and visualization. Here’s how each service is utilized:

#### Google Storage 🗄️
- **Purpose**: To store raw and processed data.
- **Usage**: The raw data from the TLC Trip Record Data is first uploaded to Google Storage. This provides a reliable and scalable storage solution for large datasets. The data stored here is accessed during the data ingestion and transformation processes.

#### Compute Engine 💻
- **Purpose**: To provide computational power for running data transformations.
- **Usage**: A Compute Engine instance is created to run the Python transformation scripts. This instance also hosts Mage, the open-source data pipeline tool, enabling the execution of data transformation workflows. Compute Engine provides the necessary resources to handle large-scale data processing efficiently.

#### BigQuery 🗃️
- **Purpose**: To serve as a scalable data warehouse.
- **Usage**: Once the data is transformed, it is loaded into BigQuery. BigQuery allows for fast querying and analysis of large datasets. It supports complex SQL queries and is optimized for performance, making it ideal for handling the processed Uber data.

#### Looker Studio 📊
- **Purpose**: To create interactive and insightful data visualizations.
- **Usage**: The final step involves creating a comprehensive dashboard in Looker Studio. Looker Studio connects to BigQuery to retrieve the processed data and provides a platform to build dynamic and interactive visualizations. This helps in deriving meaningful insights and presenting the data in an easily understandable format.

### Modern Data Pipeline Tool
- **Mage** 🚀: An open-source tool for building and managing data pipelines.
- **Usage**: Mage is used to orchestrate the data pipeline. It is installed on the Compute Engine instance and handles the workflow from data ingestion to transformation and loading into BigQuery. Mage simplifies the process of managing data workflows and ensures smooth execution of the ETL (Extract, Transform, Load) process.

## 📊 Dataset Used
We are using the **TLC Trip Record Data** which contains:
- Yellow and green taxi trip records.
- Fields include pick-up and drop-off dates/times, locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts.

### 📚 Data Dictionary
For a detailed description of the data fields, refer to the [Data Dictionary](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf).

## 🌟 Conclusion
This project showcases the integration of various modern data engineering tools and platforms to perform comprehensive data analytics. By leveraging the power of GCP, Python, and Mage, we can efficiently process large datasets and derive meaningful insights, which are then visualized using Looker Studio.
