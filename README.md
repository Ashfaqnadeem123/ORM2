# Ex02 Django ORM Web Application
## Date: 26/11/2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

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
models.py
from django.db import models
from django.contrib import admin

# create your models here
class BankLooan(models.Model):
    loan_id = odels.IntegerField(primary_key=True)
    loan_type = models.CharField(max_length=100)
    loan_amt = models.FloatFiels()
    cust_acno = models.IntegerField()
    cust_name = models.CharField(max_length=50)

class BankLoan(admin.ModelAdmin):
    list_display=('loan_id','loan_type','loan_amt','cust_acno','cust_name')
    admins.py
    from django.contrib import admin
from .models import Bankloan , BankLoanAdmin
# Register your models here.
admin.site.register(Bankloan , BankLoanAdmin)


## OUTPUT
![WhatsApp Image 2024-12-14 at 10 10 02 AM](https://github.com/user-attachments/assets/0fca0c60-49cb-4f99-83d2-e7e537b54d68)

![alt text](<Screenshot 2024-11-26 140404.png>)
![alt text](<Screenshot 2024-11-26 140541.png>)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
