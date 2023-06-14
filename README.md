# Ex02 Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a student database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![image](https://user-images.githubusercontent.com/121166004/236628802-fe4f760f-6b1b-4cd5-9c47-67d756e69c46.png)



## DESIGN STEPS : 

# STEP 1:
Clone the repository from github.

# STEP 2:
Create an admin interfacefor Django.

# STEP 3:
Create an app and edit settings.py.

# Step 4:
Makemigrations and migrate the changes.

# Step 5:
Create admin user and write pythoncode for admin and models.

# STEP 6:
Make all the migrations to 'myapp'.

# STEP 7:
Create an student database with 10 feilds using runserver command.

## PROGRAM :
```
Name : D.Vinitha Naidu
Reg No. : 212222230175
```
```
admin.py 

from django.contrib import admin
from .models import student,studentAdmin 
admin.site.register(student,studentAdmin)

models.py

from django.db import models
from django.contrib import admin
class student (models.Model):
    sid=models.CharField(max_length=28)
    name=models.CharField(max_length=30)
    regno=models.IntegerField()
    marks=models.IntegerField()
    email=models.EmailField()

class studentAdmin(admin.ModelAdmin):
    list_display=('sid','name','regno','marks','email')

```



## OUTPUT :

(![image](https://github.com/VinithaNaidu/ORM/assets/121166004/6e3a1df4-be87-4988-be72-e58a38712895)

## RESULT :
The code executed successfully.
