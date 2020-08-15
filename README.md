# Project Overview
This is the basic Django project. 
In this project, 
- I have implemented how to display values from backend server to frontend. 
- store & retrieve value from database using mysql server.

## Django Installation steps

#### Install Python
You can download the python from the following link for windows
* [Python link](https://www.python.org/downloads/windows/)

After installation check the python installed correctly or not by executing  the following command on cmd
```
python --version
```
Change the diectory where you want to install Django.Before installing Django I have created virtual environment for django so it will work on that environment only.
Following command are used for installing virtual environment
- Install virtual environment
```
pip install virtualenwrapper-win
```
- Create virtual environment
```
mkvirtualenv your-environment-name
```
- Install Django
```
pip install django
```
- Check Django installed or not
```
django-admin --version
```
- Create Django project
```
django-admin startproject your-project-name
```
- Run server form Django project
```
python manage.py runserver
```
You can run the project on 8000 port.following url for run project on browser.
```
http://127.0.0.1:8000/
```
When you want to create module in Django. you can run the following command.In python module known as app. 
```
python manage.py startapp your-app-name
```
When you close the project & again you want to work on project.First you have to start environment.
 ```
 workon your-environment-name
```
For database connection you have to install mysql client package for mysql connection.
```
pip install mysqlclient
```
Before Creating migration, register installed app in to setting.py.you can find setting.py in your main app.
- add this line to your setting.py INSTALLED_APPS array
```
'your-app-name.apps.Your-app-nameConfig',
```
After installing mysql package. You can create migration by running below command
```
python manage.py makemigrations
```
After creating migration. You can check mysql query using below command.
```
python manage.py sqlmigrate your-app-name migration-No
```
Finally migrate the file
```
python manage.py migrate
```
You can change Django admin backend.Following are the browser url for admin backend
```
http://127.0.0.1:8000/admin/
```
You can register model which will be displayed in admin backend . it will automatically create form module for this model.
```
admin.site.register(your-model-name)
```
For image handling you can install pillow package.
```
 pip install pillow
```
## Requirement
- python 3.8

## Reference
- Following are the link of telusko youtube channel
* [Telusko channel](https://www.youtube.com/watch?v=OTmQOjsl0eg)
* [mysql connection](https://medium.com/@omaraamir19966/connect-django-with-mysql-database-f946d0f6f9e3)
