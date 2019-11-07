# crudexample
## Django Sample Project

<strong>Minimum requirements:-</strong> Python 3+, Django 2.2+, WAMP/LAMP/XAMPP, MySQL 5.5+ etc.

<strong>Essentials instruction:-</strong> Installation is performed on <em>Ubuntu 18.04</em>. but if you're running a Windows system then replace <strong>python3</strong> keyword by <strong>python</strong> and run those commands.

<h4>Procedure to run project on local server (<em>Ubuntu OS</em>):</h4>


1. Download and keep this project anywhere in your file system.

2. Navigate to the project folder and open it in terminal by right clicking and selecting the option <em>Open in Terminal</em>
or directly you can navigate to the project folder by using terminal commands or <em>Windows</em> cmd.

3. If you have created <em>python environment</em> then activate it. (you can skip this step.)

4. Run <em>WAMP/XAMPP</em> or whatever you have to use <em>apache server</em> to create localhost in browser. By default <em>LAMP</em> (localhost) is always enabled in <em>Linux</em> based systems. 

5. Go to this location <em>http://localhost/phpmyadmin</em> in your browser to create a <em>new database</em> in <em>phpmyadmin</em> for your project. Create a new database and set the same name as database in <em>Django</em> settings file to use <em>mysql</em> as your database client for this project. (<em>Django</em> comes with <em>sqlite3</em> as a default database.)

    Under project folder, Go to this location <em>Project-folder/settings.py</em> (in my case - <em>crudexample/settings.py</em>) - scroll down and set the variables of <strong>'DATABASES'</strong>. <br>
    <strong>'ENGINE'</strong> is already set to <em>mysql</em>. Now set your system defined mysql credentials - <strong>'USER', 'PASSWORD'</strong> & <strong>'NAME'</strong>. <em>'NAME'</em>n will define database name here.

6. Now run these commands in your <em>Linux</em> terminal or <em>Windows</em> cmd -

    <em>python3 -m pip install --upgrade pip</em>
    <br><em>pip install django</em>
    <br><em>pip install mysqlclient</em>
    <br><em>python3 -m pip install mysql-connector</em>

    It will <em>upgrade pip</em> (if your pip version is old), install <em>Django</em>, install <em>mysql-client</em> or <em>python-mysql</em> connectivity. 

7. Run these commands in terminal to update <em>Django</em> database in <em>mysql</em> - 

    <em>python3 manage.py makemigrations</em>
    <br><em>python3 manage.py migrate</em>

    It will migrate the initial <em>Django</em> installation tables for the first-time use it on local server. Later you can use these commands if you need to update database tables in <em>Django</em> applications.

8. Run this command in terminal <strong>python3 manage.py runserver</strong> to initialize localhost. It will create a localhost server with any random port. <em>i.e. 80*</em>

    Note:- If you are using <em>Windows</em> OS then use <strong>python manage.py runserver</strong> command in cmd.

9. Right click and open the localhost path <em>http://127.0.0.1:8000/</em>
   Sometimes port can be changed but it will be similar to 80*. this will open and run the project in a browser window.

10. To quit or terminate the localhost, press <strong>ctrl+c</strong> in terminal window.

11. You can access the <em>admin panel</em> by appending <strong>/admin</strong> keyword in localhost url like - <em>http://127.0.0.1:8000/admin/</em>

# <h4>Support</h4>

To download and install Python - <em>https://www.python.org/downloads/</em>
<br>Python documentation - <em>https://docs.python.org/3/</em>

To download and install Django - <em>https://www.djangoproject.com/download/</em>
<br>Django documentation - <em>https://docs.djangoproject.com/en/2.2/</em>

# <h3>Project Description</h3>

This project is just for a demo purpose to perform basic CRUD operations at Django front-end.

