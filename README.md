# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
   Clone the repository from github

### STEP 2:
   Create an admin page for Django.

### STEP 3:
   create an app and edit settings.py

### STEP 4:
   Makemigration and migrate the changes.

### STEP 5:
   Create admin user and write python code for admin and models

### STEP 6:
   Make all the migration to my app

### STEP 7:
   Create a students database with 10 fields using runservercommand
admin.py

### PROGRAM:
from django.contrib import admin
from .models import Student,StudentAdmin
admin.site.register(Student,StudentAdmin)

models.py

from django.db import models
from django.contrib import admin

class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()


class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')

## OUTPUT



![ex200](https://github.com/22009058/ORM/assets/121917232/7b17769a-3754-4869-96be-8fc2efd55d71)


## RESULT
The program for creating a studentdatabase using ORM is executed successfully.
