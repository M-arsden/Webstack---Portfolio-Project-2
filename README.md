# E-Learning System

### Description 
This is video based learning system to assist the students, like those attending ALX school, to get expert or mentor lectures easily. To easily group the course videos, the databases are categorized into contents, modules, and courses. The course can have multiple modules and the same module can have multiple contents. The courses have their reference tab to hold any books or documents to help the students to get references on the specific subject. 

### About Me 
My name is Marsden Abucheri, ALX graduate with software engineer, backend specialized. I do have experience in Django and I did more than 3 projects, including this one, with MySQL database and HTML, CSS & some JavaScript. I am studying Computer Science to be graduated on 2023. I'm also have BA degree in Logistics and Supply Chain Management with 5+ years experience as Procurement Officer. I love coding and I want to be web and application developer. I’m passionate about creating truly beautiful, efficient and problem solving softwares. 


### Installation
The first thing to do is to clone the repository:



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
### What This Project Accomplished
+ Categorizing the course in to module and contents 
+ Attaching multiple reference documents for a given courses 
+ Multiple forms on single page 
+ Filtering the course by available category using checkbox and  
search by all mechanizm. 
+ Adding detail of the courses using rich text  
+ Rendering the pages using extend mechanizm  
+ Giving authority for the pages as role of the user

### What can be improve? 
+ Marking the content of the course and the course it self complete 
+ Issuing certificates upon completion 
+ Add review futures 
+ Add question and answer platform

### Related projects
> Database Management System for Orthodox church Sunday school.

> [Online Library for ALX Foundation Portfolio Project](https://github.com/MikiyasA/Online_Library-ALX_Foundation_Portfolio_Project)

### Licensing
****Free Software, developed for portfolio project****
