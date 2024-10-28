# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![alt text](<Screenshot 2024-10-26 145443.png>)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
```
models.py 

from django.db import models
from django.contrib import admin
class people(models.Model):
       Name=models.CharField(max_length=15)
       Aadharno=models.IntegerField(primary_key="Aadharno")
       address=models.CharField(max_length=20)
       loanamt=models.IntegerField()
       Email=models.EmailField()
class peopleAdmin(admin.ModelAdmin):
       list_display=('Name','Aadharno','address','loanamt','Email')

admin.py

from django.contrib import admin
from .models import people,peopleAdmin
admin.site.register(people,peopleAdmin)
```

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM



## OUTPUT

![alt text](<Screenshot (6).png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
