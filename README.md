# <h2>crudexample<h2> 
## Django Sample Project

<strong>Minimum requirements:-</strong> Python 3+, Django 2.2+, WAMP/LAMP/XAMPP, MySQL 5.5+ etc.

<strong>Essentials instruction:-</strong> Installation is performed on Ubuntu 18.04. but if you're running a Windows system then use <strong>'python'</strong> keyword in below listed commands. If you're running a Linux system then replace <strong>'python'</strong> keyword by <strong>'python3'</strong> and run those commands.

<h4>Procedure to run project on local server (Ubuntu OS):</h4>


1. Download and keep this project anywhere in your file system.

2. Navigate to the project folder and open it in terminal by right clicking and selecting the option <em>"Open in Terminal"</em>
or directly you can navigate to the project folder by using terminal commands or windows cmd.

3. If you have created python environment then activate it else you can skip this step.

4. Run <em>WAMP/XAMPP</em> or whatever you have to use apache server to create localhost. By default LAMP (localhost) is always enabled on Linux systems. 

5. Go to this location 'http://localhost/phpmyadmin' in your browser to <em>create a new database</em> in phpmyadmin for your project. Create a new database and set the same name as database in Django settings file to use mysql as your database client for this project. (Django comes with <em>sqlite3</em> as a default database)

    Under project folder, Go to this location <em>Project-folder/settings.py</em> (in my case - <em>crudexample/settings.py</em>) - scroll down and set the variables of <strong>'DATABASES'</strong>. <br>
    <strong>'ENGINE'</strong> is already set to mysql. Now set your system defined mysql credentials - <strong>'USER', 'PASSWORD' & 'NAME'</strong>. <em>'NAME'</em>n will define database name here.

6. Now run these commands in your windows cmd or linux terminal -

    <em>python3 -m pip install --upgrade pip</em>
    <br><em>pip install django</em>
    <br><em>pip install mysqlclient</em>
    <br><em>python3 -m pip install mysql-connector</em>

    It will upgrade pip (if your pip version is old), install Django, install mysql-client or python-mysql connectivity. 

7. Run these commands in terminal to update mysql database with Django - 
    <br><em>python3 manage.py makemigrations</em>
    <br><em>python3 manage.py migrate</em>

8. Run this command in terminal <strong>python3 manage.py runserver</strong> to initialize localhost. It will create a localhost server with any random port. i.e. 80*
If you are using Windows OS then use <em>python manage.py runserver</em> command in cmd.

9. Right click and open the localhost path http://127.0.0.1:8000/ 
   Sometimes port can be changed but it will be similar to 80*. this will open and run the project in a browser window.

10. To quit or terminate the localhost, press <strong>ctrl+c</strong> in terminal window.

11. You can access the admin panel by appending <em>/admin</em> keyword in localhost url like:- http://127.0.0.1:8000/admin/

# <h4>Support</h4>

To download and install Python - <em>https://www.python.org/downloads/</em>
<br>Python documentation - <em>https://docs.python.org/3/</em>

To download and install Django - <em>https://www.djangoproject.com/download/</em>
<br>Django documentation - <em>https://docs.djangoproject.com/en/2.2/</em>

# <h3>Project Description</h3>

This project is just for a demo purpose to perform basic CRUD operations at Django front-end.

