# ETL-Airflow-pipeline-Open-Weather-Map-API
build and automate a python ETL pipeline with airflow on AWS EC2


![Screen Shot 2023-12-30 at 12 54 56 PM](https://github.com/devaa07/ETL-Airflow-pipeline-Open-Weather-Map-API/assets/126756574/232cac61-58a5-45bf-a429-a658eef370ce)


# Step 1: Create AWS EC2 instance with t2.medium as the recommended instance type

# Step 2: Insall the required modules/packages
          sudo apt update
          sudo apt install python3-pip
          sudo apt install python3.10-venv
          python3 -m venv airflow_venv
          sudo pip install pandas
          sudo pip install s3fs
          sudo pip install apache-airflow

# Step 3: Create the DAG and write the required tasks Refer weather_dap.py file in the code repo

# Step 4: Configure the aws credentials 
          sudo apt  install awscli
          aws configure
          aws sts get-session-token

# Step 5: Add the aws_credentails in the code and trigger the DAG in the airflow UI

<img width="800" alt="Screen Shot 2023-12-30 at 12 52 35 PM" src="https://github.com/devaa07/ETL-Airflow-pipeline-Open-Weather-Map-API/assets/126756574/e237e5af-d10f-4671-8cfa-8c3d0fa04551">

          
# Step 6: See the resultant csv file and we are done!!

<img width="674" alt="Screen Shot 2023-12-30 at 12 56 02 PM" src="https://github.com/devaa07/ETL-Airflow-pipeline-Open-Weather-Map-API/assets/126756574/4381192b-01dd-4003-a98b-7feede1735af">



