# mini
 A mini app to log and display the time we need to make the cages,at different workstations.
 ![image](https://github.com/jpriyam/mini/blob/master/mini.gif)
 
 
 
1) Install Python (3.6 or 3.7) 
2) Install git bash on the laptop
3) Clone the repository .
4) There is a file called requirements.txt use the command 
pip install -r requirement.txt
5) In settings.py,make the following changes:
DATABASES = {
    'default': {
        'ENGINE' : 'django.db.backends.mysql',
        'NAME' : '<db_name>',
        'HOST' : '127.0.0.1',
        'PORT' : '3306',
        'USER' : ' <db_user>',
        'PASSWORD' : '<db_user_password> ',
    }
}

6) Create a database in the with the same name in mysql
7) Create a super user with the following commands 
python manage.py createsuperuser
Enter your name and password.
8) Then run 
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
In that order 

(In case of an error in manage.py migrate try running 
Python manage.py migrate --run-syncdb to connect to the database)
