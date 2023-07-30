With docker 
cd into Location file 
docker-compose build
docker-compose up -d db
docker-compose up web
docker exec web_container_name python manage.py migrate
Navigate to localhost:8085/places This page has leaflet map with search functionality 
For Swagger UI localhost:8085/swagger You can find all the relevant endpoints here 
Run Pytest command to run tests

Without Docker 
Download postgredb and make database with config present in settings.py 
database name : db user : postgres password: postgres PORT:5432
Clone the entire repository 
cd into Location 
Create Virtual enviroment 
Pip install -r requirements.txt 
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
Navigate to localhost:8085/places This page has leaflet map with search functionality 
For Swagger UI localhost:8085/swagger You can find all the relevant endpoints here 
Run Pytest command to run tests

Find Screenshots for Application in ScreenShots for Application Folder

