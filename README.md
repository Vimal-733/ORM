# Ex02 Django ORM Web Application
# Date:
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
models.py
```
from django.db import models
from django.contrib import admin

class Book(models.Model):
    book_no = models.CharField(max_length=100, primary_key=True)
    book_name = models.CharField(max_length=100)
    name = models.CharField(max_length=100)
    mobile_no = models.CharField(max_length=15)
    email = models.EmailField()
    aadhar_no = models.CharField(max_length=12)
    

class BookAdmin(admin.ModelAdmin):
    list_display = ('book_no', 'book_name', 'name', 'mobile_no', 'email','aadhar_no')
```
admins.py
```
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)
```
# OUTPUT
![image](https://github.com/user-attachments/assets/a0a5097c-cb5f-46ae-bffa-5c2cfd4d05fb)

![image](https://github.com/user-attachments/assets/1662da9b-1b1f-4d00-8433-fd2493df3e0d)
![image](https://github.com/user-attachments/assets/d559d167-1510-4dac-a62a-694999c5dc9e)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
