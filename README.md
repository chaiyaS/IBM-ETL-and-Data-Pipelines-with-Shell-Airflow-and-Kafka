# IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka
# Description
For this project, the ELT is performed with the support of Airflow and Kafka. Assume you are a data engineer at a data analytics consulting company. You have been assigned to a project that aims to de-congest the national highways by analyzing the road traffic data from different toll plazas. Each highway is operated by a different toll operator with different IT setup that use different file formats.
In the first Hands-on lab your job is to collect data available in different formats and, consolidate it into a single file. As a vehicle passes a toll plaza, the vehicle's data like vehicle_id,vehicle_type,toll_plaza_id and timestamp are streamed to Kafka. In the second Hands-on lab your job is to create a data pipe line that collects the streaming data and loads it into a database.

# Tasks and Solutions
- Task 1.1: Define DAG arguments (2pts)

![01 dag_args](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/2d795dcb-0e52-4ded-96e1-3c02a52fd8b6)

- Task 1.2: Define the DAG (2pts)

![02 dag_definition](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/56fd7682-8078-4e5b-9c4e-e21a4b5bea78)

- Task 1.3: Create a task to download data (2pts)
  
![03 unzip_data](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/96c7a3e7-5ff9-4e82-88ef-4ec7b0cfdcf5)

- Task 1.4: Create a task to extract data from csv file (2pts)

![04 extract_data_from_csv](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/0750667c-a0a2-4ce1-9757-578b8580b0c0)

- Task 1.5: Create a task to extract data from tsv file (2pts)

![05 extract_data_from_tsv](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/e37336a6-b914-469c-b49e-fa417ed12c81)

- Task 1.6: Create a task to extract data from fixed width file (2pts)

![06 extract_data_from_fixed_width](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/4e1b5ed2-dd1f-40a7-b498-35fdf599da02)

- Task 1.7: Create a task to consolidate data extracted from previous tasks (2pts)

![07 consolidate_data](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/ba8c7c79-acaf-42d8-860b-ec0f7d830325)

- Task 1.8: Transform the data (2 pts)

![08 transform](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/2d2a7245-65ff-494a-9663-4da553e98a7e)

- Task 1.9: Define the task pipeline (1pt)

![09 task_pipeline](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/6674c21d-45ca-4579-969b-c9a7f47f3e2b)

- Task 1.10: Submit the DAG (1pt)

![10 submit_dag](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/52c6cb4e-2de1-4f1a-9292-a3112cd23a7b)

- Task 1.11: Unpause the DAG (1pt)

![11 unpause_dag](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/91aeff55-ab5c-430a-a86f-c7e58b4bcc9c)

- Task 1.12: Monitor the DAG (1pt)
  
  If you try to extract or write file to aipflow/dasg/... you need to using by ls -l (your directory) to check your directory that they can permission to write into your directory. if can not write, you need to use chmod 777 to that directory. After that, you can write anything to that directory.

  ![12 monitor the DAG](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/000da55e-79aa-405b-983d-4703cd254504)

- Task 2.1: Start Zookeeper (1pt)

![01 start_zookeeper](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/52312a9c-e9d3-4099-98ae-bde0f8b81d5e)

- Task 2.2: Start Kafka server (1pt)

![02 start_kafka](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/ecfca1f7-ab5f-4b1a-a662-09ad1fb120ce)

- Task 2.3: Create a topic named toll (1pt)

![03 create_toll_topic](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/4969c5dd-85ca-49a0-bbd9-bfabd1891fa4)

- Task 2.4: Download the Toll Traffic Simulator (1pt)

![04 configure_simulator](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/b193b02c-d3af-45a2-b7fe-04e94f7d049f)

- Task 2.5: Configure the Toll Traffic Simulator (1pt)

![05 download_simulator](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/05bae677-bc5d-4d0e-af0c-6f5e0bd11e1b)

- Task 2.6: Run the Toll Traffic Simulator (1pt)

![06 simulator_output](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/2cee812d-70c4-473f-9325-d5eee86ec4f5)

- Task 2.7: Configure streaming_data_reader.py (2pts)

![07 streaming_reader_code](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/7457d878-b835-4a3b-80f4-e119ce82d6e5)

- Task 2.8: Run streaming_data_reader.py (1pt)

![08 data_reader_output](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/968d6476-d100-4423-b1c1-83f86f85b13b)

- Task 2.9: Health check of the streaming data pipeline (1pt)
  
  ![09 output_rows](https://github.com/chaiyaS/IBM-ETL-and-Data-Pipelines-with-Shell-Airflow-and-Kafka/assets/142322529/9ed49371-ac9e-4dd2-b590-f3a012dcadbc)
