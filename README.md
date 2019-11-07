# <h2>crudexample<h2> 
##(Django Sample Project)
note: work in progress

Minimum requirements: Python 3+, Django 2.2+, MySQL 5.5+ etc.

Essentials instruction - Installation is performed on Ubuntu 18.04. but if you're running a Windows system then use 'python' keyword in below listed commands. If you're running a Linux system then replace 'python' keyword by 'python3' and run those commands.

<h4>Procedure to run project on local server (Ubuntu OS):</h4>


1. Download and keep this project anywhere in your file system.

2. Navigate to the project folder and open it in terminal by right clicking and selecting the option "Open in Terminal"
or directly you can navigate to the project folder by using terminal commands or windows cmd.

3. If you have created python environment then activate it else you can skip this step.

4. Run WAMP/XAMPP or whatever you have to use apache server to create localhost. By default LAMP (localhost) is always enabled on Linux systems. 

5. Go to this location 'http://localhost/phpmyadmin' in your browser to create a new database in phpmyadmin for your project. Create a new database and set the same name as database in Django settings file to use mysql as your database client for this project. (Django comes with sqlite3 as a default database)

Under project folder, Go to this location Project-folder/settings.py (in my case - crudexample/settings.py) - scroll down and set the variables of 'DATABASES'. 
'ENGINE' is already set to mysql. Now set your system defined mysql credentials - 'USER', 'PASSWORD' & 'NAME'. 'NAME' will define database name here.

6. Now run these commands in your windows cmd or linux terminal -

python3 -m pip install --upgrade pip
pip install django
pip install mysqlclient
python3 -m pip install mysql-connector

It will upgrade pip (if your pip version is old), install Django, install mysql-client or python-mysql connectivity. 

6. Run these commands in terminal to update mysql database to set-up it for Django - 
python3 manage.py makemigrations
python3 manage.py migrate

6. Run this command in terminal "python3 manage.py runserver" to initialize localhost. It will create a localhost server with any random port. i.e. 80*
If you are using Windows OS then use "python manage.py runserver" command in cmd.

7. Right click and open the localhost path http://127.0.0.1:8000/ 
   Sometimes port can be changed but it will be similar to 80*. this will open and run the project in a browser window.

8. Terminate the localhost by pressing ctrl+c in terminal window.

9. You can access the admin panel by appending '/admin' keyword in localhost url like:- http://127.0.0.1:8000/admin/

# <h4>Support</h4>

To download and install Python - https://www.python.org/downloads/
Python documentation - https://docs.python.org/3/

To download and install Django - https://www.djangoproject.com/download/
Django documentation - https://docs.djangoproject.com/en/2.2/

# <h3>Project Description</h3>

This project is just for a demo purpose to perform basic CRUD operations at Django front-end.

