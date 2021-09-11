# Yuva Parivartan- NGO

![](https://img.shields.io/github/license/CybSec-NITW/WeaponHEX)
![](https://img.shields.io/pypi/pyversions/django.svg)

- Yuva Parivartan mainly focuses on giving a second chance to the  school dropouts and underpriviledged students.
- Data collected by the YuvaParivartan is spread across different  databases for students, employees, audit scores. 
- **ISSUE:** The main problem faced is managing data on a single platform and for quick accessibility, decision-making and instant results for availability of data anytime and anywhere.
- **SOLUTION:** Our platform allows consolidation of data from different sources ( .csv file with the specified fields) and generates a category wise summary for the following categories:    
	* HR
	* Impact Support
	* Audit

- The .csv file made using the specified fields and data inserted will serve as a data blueprint to generate categories and other data points.
- The Admin site offers role-based authorization that segregates users based on login ID's into Admin that can carry out tasks like manage users.
- The .csv file(created by the test data) has been presented in form or Bar graphs, Line graphs and scatter plots for easy data visualization. 
- The reports are generated via different systems and pulled out in the form of excel file using the test data added.

## Source code of the project-

## Instructions

Make sure you have Git and Python installed on your machine. If not, you can download and install them from here: https://git-scm.com/downloads https://www.python.org/downloads/

Open a terminal and change current directory to your dev or projects folder.

Then follow these steps
```
$ pip install virtualenv
$ mkdir codeforgood
$ cd codeforgood
$ git clone https://github.com/IndiaCFG3/team-38.git .
// A login would be required since it is a private repository
$ virtualenv -p python3 .
$ .\Scripts\activate                               #For MAC/Linux -> . bin/activate
(codeforgood) $ pip install -r requirements.txt
(codeforgood) $ cd src
(codeforgood) $ python manage.py makemigrations #For MAC/Linux -> python3 manage.py makemigrations
(codeforgood) $ python manage.py migrate        #For MAC/Linux -> python3 manage.py migrate
(codeforgood) $ python manage.py runserver      #For MAC/Linux -> python3 manage.py runserver
It will deploy the website on your localhost https://127.0.0.1:8000
```

## Admin login

Django provides a default admin interface which can be used to perform create, read, update and delete operations on the models and manage users directly.

```
Go to directory containing manage.py file and enter the following command to create a new superuser

$ python manage.py createsuperuser

Enter the details. After successful creation open https://127.0.0.1:8000/admin and use your login credentials.
```

PS : You can use git GUI clients such as GitKraken or SourceTree to manage your projects.

## Models:
- **HR:**
```
employee_id-charstring
employee_name-string
employee_phone-integer
employee_email-charstring
manager_id-integer
doj-date
employee_status-string
leaves_applied-integer 
```

- **Audit:**
```
center_id - charstring
city - string
student_count - integer
staff_count - integer
student_joined - integer
students_completed - integer
students_dropped - integer
rating -integer 
```

- **For support_team :**
```
id - charstring
name - string
email - email
batch_id - integer
enrolled_course - string
enrolled_date - date
attendance - float
course_status - boolean
placement_status - boolean
```

## Implementation
- ![yp1](https://user-images.githubusercontent.com/60674228/132943910-675a4810-fa27-4d61-a958-4cd874ff3978.PNG)

- ![yp2](https://user-images.githubusercontent.com/60674228/132943916-65274b8b-1645-4fdd-bd07-cb4245a5e214.PNG)

- ![yp3](https://user-images.githubusercontent.com/60674228/132943923-e0bd061a-c54c-48f3-906e-2b2c673ee3dd.PNG)

- ![yp4](https://user-images.githubusercontent.com/60674228/132943932-d2ae5d86-0a51-42f9-976c-408dca4248ab.PNG)


#### Video link: 
https://drive.google.com/file/d/17UGILCaLmBN1MEbtNulJPfmPudNSZ3go/view?usp=sharing
