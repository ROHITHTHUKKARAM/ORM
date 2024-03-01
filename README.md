# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Alt text](<Screenshot 2024-02-29 140553.png>)

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
class library(models.Model):
      serielno=models.IntegerField(primary_key=True);
      book_name=models.CharField(max_length=20);
      authorname=models.CharField(max_length=20);
      subject=models.CharField(max_length=50);
      publisher=models.CharField(max_length=10);
class libraryAdmin(admin.ModelAdmin):
      list_display=("serielno","book_name","authorname","subject","publisher");

admin.py
from django.contrib import admin
from.models import library,libraryAdmin
admin.site.register(library,libraryAdmin)
```
## OUTPUT

![Alt text](<Screenshot 2024-02-29 142430.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
