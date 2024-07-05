**Prerequisites:**

  First, make sure you have installed Docker Desktop and Visual Studio.

**Install Apache Airflow with Docker:**

  Create a folder materials in your Documents
  
  In this folder, download the following file: docker compose file
  
  If you right-click on the file and save it, you will end up with docker-compose.yaml.txt. Remove the .txt and keep docker-compose.yaml
  
  Open your terminal or CMD and go into Documents/materials
  
  Open Visual Studio Code by typing the command: code .

  Right click below docker-compose.yml and create a new file .env (don't forget the dot before env)

  In this file add the following lines
  '''
  AIRFLOW_IMAGE_NAME=apache/airflow:2.4.2
  AIRFLOW_UID=50000
  ''' and save the file

  Go at the top bar of Visual Studio Code -> Terminal -> New Terminal

  In your new terminal at the bottom of Visual Studio Code, type the command docker-compose up -d and hit ENTER.

  You will see many lines scrolled, wait until it's done. Docker is downloading Airflow to run it. It can take up to 5 mins depending on your connection.

  Open your web browser and go to localhost:8080
  login and password are "airflow".

for trouble shoot
 command:- docker-compose ps
