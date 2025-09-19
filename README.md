# Ex02 Django ORM Web Application
## Date:19.09.2025 

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## Entity Retionship Diagram
![WhatsApp Image 2025-09-13 at 11 18 52 AM](https://github.com/user-attachments/assets/3a80f404-5db2-47af-9731-a2de86a9d5ca)


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
from .models import Car

admin.site.register(Car)

models.py
from django.db import models

class Car(models.Model):
    car_id = models.AutoField(primary_key=True)
    brand = models.CharField(max_length=100)
    model = models.CharField(max_length=100)
    year = models.IntegerField()
    price = models.FloatField()

    def _str_(self):
        return f"{self.brand} {self.model}"


```
## OUTPUT
![alt text](<Screenshot 2025-09-19 085926.png>)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
