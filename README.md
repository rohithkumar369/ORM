# Ex02 Django ORM Web Application
## Date: 15-04-2025
## Name:s.rohith kumaar
## registration number:212224240153

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
## models.py
```
from django.db import models
from django.contrib import admin
class Movie(models.Model):
mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField()
class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','mname','collection','year','rating')
```
## admin.py
```
from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)
```

## OUTPUT

Include the screenshot of your admin page.
![433032746-58adb5eb-db97-416f-8c2c-84da4951b1f2](https://github.com/user-attachments/assets/4fb9a9ea-03c8-47a9-906d-96484776775c)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
