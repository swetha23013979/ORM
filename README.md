# Ex02 Django ORM Web Application
## Date: 11/3/24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
<img width="451" alt="er diagram booklist ss" src="https://github.com/swetha23013979/ORM/assets/153823422/b7fb51db-3007-4295-beca-dac589b5f5a5">



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
class Book(models.Model):
  Book_id=models.IntegerField(primary_key=True);
  Book_author=models.CharField(max_length=20);
  Book_name=models.CharField(max_length=50);
  publication=models.DateField();
  price=models.IntegerField();
class BookAdmin(admin.ModelAdmin):
  list_display=("Book_id","Book_author","Book_name","publication","price");

admin.py
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
Include your code here

```

## OUTPUT
<img width="958" alt="booklist ss" src="https://github.com/swetha23013979/ORM/assets/153823422/d582522c-2b48-4dbb-b792-91add67e85fd">




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
