# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


![Screenshot 2024-03-21 142803](https://github.com/R01ty/ORM/assets/142526219/95969447-81f2-430b-a6f0-9a38dfff078a)

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
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)

models.py

from django.db import models
from django.contrib import admin
class footballplayer (models.Model):
    name=models.CharField(max_length=15)
    weight=models.IntegerField()
    age=models.IntegerField()
    members=models.CharField(max_length=20)
    experiance=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('name','weight','age','members','experiance')


```

## OUTPUT

![image](https://github.com/Thajesh2/ORM/assets/139841959/6baf85fe-8fb3-48b9-9101-028e887c62e3)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
