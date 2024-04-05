# Ex02 Django ORM Web Application
## Date: 05/04/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

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
Execute Django admin and create details for 10 books

## PROGRAM

```
models.py
from django.db import models

# Create your models here.

from django.contrib import admin

class Bookdetails(models.Model):
   Studentname=models.CharField(max_length=20);
   Regno=models.IntegerField();
   BookName=models.CharField(max_length=50);
   AuthorName=models.CharField(max_length=50);
   BookNo=models.IntegerField(primary_key=True);
   YearofRelease=models.DateField();
   
class BookdetailsAdmin(admin.ModelAdmin):
   list_display=("Studentname","Regno","BookName","AuthorName","AuthorName","BookNo","YearofRelease");

admin.py

from django.contrib import admin

# Register your models here.
from .models import Bookdetails,BookdetailsAdmin
admin.site.register(Bookdetails,BookdetailsAdmin)
```

## OUTPUT

![Screenshot 2024-04-05 225414](https://github.com/selvasachein/ORM/assets/144979117/26523900-9fe1-46ff-bee9-e8259f9fbcfb)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
