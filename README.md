# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot from 2024-01-02 18-02-06](https://github.com/Rxhith1205/django-orm-app/assets/147473311/e52ddd9e-cd73-4993-9a7a-73f9ef29bc46)


## DESIGN STEPS

### STEP 1:
close the empty repository from gitup
### STEP 2:
under the directory Dataproject install a Django project named 'myapp'.check database engine
### STEP 3:
write our code in models.py and setting.py and admin.py.Run Django Project
Write your own steps

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

modles.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
## OUTPUT
![Untitled](https://github.com/Rxhith1205/django-orm-app/assets/147473311/1a4b815e-0645-4a7c-be9e-222f03eb9069)


## RESULT
The program is executed succesfully
