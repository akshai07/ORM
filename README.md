# Ex02 Django ORM Web Application
## Date: 20-03-2024
## Name: Akshai Khanna D
## Reg.no: 212223040010
## Dept: CSE

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![320077298-28e98abf-2f0c-4c2a-b433-190c6e6592fe](https://github.com/akshai07/ORM/assets/152007451/a12202fa-5798-47c1-94cd-bdee34288cc0)

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
```
admin.py:
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
```

## OUTPUT

 ![320069592-ce7ec008-de1f-44db-8594-39060bfd7381](https://github.com/akshai07/ORM/assets/152007451/f158e437-129f-49ce-af39-3092dd399d67)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
