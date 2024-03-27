# Ex02 Django ORM Web Application
## Date: 18.03.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

<img width="576" alt="screen shot paint" src="https://github.com/sreevarshad/ORM/assets/128129573/d9a8ca5c-5400-4632-ac01-de3ae6e38e17">

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
admin.py

from django.contrib import admin
from .models import Book_DB,Book_DBAdmin
admin.site.register(Book_DB,Book_DBAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book_DB(models.Model):
      sno=models.IntegerField(primary_key="sno")
      name=models.CharField(max_length=50)
      author=models.CharField(max_length=70)
      price=models.IntegerField()
      publisher=models.CharField(max_length=60)

class Book_DBAdmin(admin.ModelAdmin):
    list_display=("sno","name","author","price","publisher")

```
## OUTPUT

<img width="956" alt="EXorm-1" src="https://github.com/sreevarshad/ORM/assets/128129573/663ab3e4-a04c-4162-a90a-78a272b8ea7b">


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
