# Ex02 Django ORM Web Application
## Date: 14/09/2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
#FROM Admin.py
from django.contrib import admin
from .models import Student,StudentAdmin
# Register your models here.
admin.site.register(Student,StudentAdmin)

#FROM Models.py
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referenceno=models.CharField(primary_key=True,max_length=20,help_text="referenceno")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()
    mobileno=models.IntegerField()
class StudentAdmin (admin.ModelAdmin):
    list_display=('referenceno','name','age','email','mobileno')
```

## OUTPUT
![image](https://github.com/Kishorekumar22060/ORM/assets/141472136/4f2c4c40-f25e-4133-b523-30d1138d7513)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
