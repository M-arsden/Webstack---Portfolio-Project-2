# E-Learning System

### Introduction
This is video based learning system to assist the students, like those attending ALX school, to get expert or mentor lectures easily. To easily group the course videos, the databases are categorized into contents, modules, and courses. The course can have multiple modules and the same module can have multiple contents. The courses have their reference tab to hold any books or documents to help the students to get references on the specific subject. 

+ [LinkedIn](https://www.linkedin.com/in/mikiyas-adere-373258225) - Mikiyas Adere

### Installation
The first thing to do is to clone the repository:

>  $ https://github.com/MikiyasA/ALX-Webstack-Portfolio_Project_E-Learning_System


Then make sure your machine is capable to run the code. The below command is for Linux OS

```sh
sudo apt-get install python3.*
sudo apt install python3-django
pip install django-crispy-forms
pip install django-ckeditor
```

Change your directory to the folder that holds manage.py file. After that, createsuperuser to have admin write and access admin page.
```sh
python3 manage.py createsuperuser
"""Then follow the stapes and provide the information needed."""
```

Then, it is time to run the program. Just enter the below command without changing your directory.

```sh
python3 manage.py runserver
"If you want to run it with different port, use the below"
python3 manage.py runserver <port_no_you_want>
```
And navigate to `http://127.0.0.1:8000/`. or `http://127.0.0.1:<port_no_you_enter>/`

#### Setting 

You can deploy this system with two different database system, MySql or sqlite. Just open setting.py file located in `.../elearning` directory make adjustment as be below.

`To run with sqlite database, make sure to uncomment the below code and comment any code line start with "DATABASES = {"`
```
 DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
 }

 ```
To run with MySql database, make sure to uncomment the below code and comment any code line start with "DATABASES = {"
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': '<name_of_your_schema>',
        'USER': '<user_name_with_write_privilege>',
        'PASSWORD': '<password>',
    }
}
```

### Related projects
> Database Management System for Orthodox church Sunday school.
> Online Library for ALX Foundation Portfolio Project

### Licensing
****Free Software, developed for portfolio project****
