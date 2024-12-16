# Ex02 Django ORM Web Application
# Date:07.12.20224
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

# admin.py
```
from django.contrib import admin

from .models import Bankloan,BankloanAdmin

admin.site.register(Bankloan,BankloanAdmin)
```
# models.py
```

from django.db import models

from django.contrib import admin

class Bankloan(models.Model):

  date_of_birth=models.DateField(default=0)

  name=models.CharField(max_length=70,default=0)

  age=models.IntegerField(default=0)

  customerid=models.IntegerField(primary_key="customerid",default=0) 

  mail=models.CharField(max_length=70,default=0)


class BankloanAdmin(admin.ModelAdmin):
 list_display=('date_of_birth','name','age','customerid','mail')
```

# OUTPUT
![Screenshot 2024-12-16 100359](https://github.com/user-attachments/assets/24189cf5-158b-47b7-b8e6-026662ff729f)

![image](https://github.com/user-attachments/assets/1697ea1d-96c0-446c-8874-46e19069f19d)



# RESULT
Thus the program for creating a database using ORM hass been executed successfully
