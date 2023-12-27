# TheVoice-PySpark
 The voice ETL using pyspark

<b>Introduction</b>

The motivation for this project is to develop an ETL process using pyspark and develop a DWH schema.
I used TheVoice db attached in the project files.
S2T mapping requirements attached in the project files.


<b>Project Description </b>

In this project i used three stages to build the DWH:

    * 1_mrr - In this stage all the data was read from parquet files and loaded into spark dataframes. 

    * 2_stg - This stage is the transformation stage where i used the source tables to create the tables in the warehouse according to S2T file.

    * 3_dwh - This is the final stage where i have implemented incrmental load for each table using its key

    ** I decided not to develop the DimTime table since the the timestamp was 00:00:00
    
