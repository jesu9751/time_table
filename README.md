# Ex03 Time Table
# Date:28.11.2025
# AIM
To write a html webpage page to display your slot timetable.

# ALGORITHM
## STEP 1
Create a Django-admin Interface.

## STEP 2
Create a static folder and inert HTML code.

## STEP 3
Create a simple table using `<table>` tag in html.

## STEP 4
Add header row using `<th>` tag.

## STEP 5
Add your timetable using `<td>` tag.

## STEP 6
Execute the program using runserver command.

# PROGRAM

urls.py
```
from django.contrib import admin
from django.urls import path
from slotapp import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('tt/', views.slot)
]
```

views.py
```
from django.shortcuts import render

def slot(request):
    return render(request,'slot.html')
```

slot.html
```
<html>
    <head>
        <title>slot</title>
        <style>
            table,th,td{
                text-align: center;
                border-style: double;
                margin-left: auto;
                margin-right: auto;
            }
        </style>
    </head>
    <body>
        <img src="saveetha.jpg" width="40%" height="20%" style="margin-left: 30%; margin-right:60%;">
     <br>
     <br>
        <table style="background-color: hsl(160, 100%, 75%);" cellspacing="2px" cellpadding="2px" width="50%" height="40%">
            <caption>SLOT TIME TABLE-JESU JOYAL(25019126)</caption>
        

        <tr style="background-color: yellow;">
            <th style="background-color: yellow;">Day/Time</th>
            <th style="background-color: yellow;">Monday</th>
            <th style="background-color: yellow;">Tuesday</th>
            <th style="background-color: yellow;">Wednesday</th>
            <th style="background-color: yellow;">Thursday</th>
            <th style="background-color: yellow;">Friday</th>   
        </tr>
        <tr>
            <td style="background-color: yellow;">8AM-10AM</td>
            <td colspan="3">WEB</td>
            <td colspan="2" >FREE SLOT</td>
        </tr>
        <tr>
            <td style="background-color: yellow;">10AM-12PM</td>
            <td>COM ENG</td>
            <td>PYTHON</td>
            <td colspan="2">FREE SLOT</td>
            <td>COM ENG</td>
        </tr>
        <tr>
            <td style="background-color: yellow;">12PM-1PM</td>
            <td colspan="5">LUNCH BREAK</td>    
        </tr>  
        <tr>
            <td style="background-color: yellow;">1PM-3PM </td>
            <td>WEB</td>
            <td>FREE SLOT</td>
            <td>MENTOR MEET</td>
            <td>FREE SOLT</td>
            <td>WEB</td>
        </tr>
        <tr>
            <td style="background-color: yellow;">3PM-5PM</td>
            <td>FREE SLOT</td>
            <td colspan="3" >PYTHON</td>
            <td>FREE SLOT</td>  
        </tr>        
        </table>
        <br>                                                        
        <table style="border: 4;" style="border: double;" cellpadding="10" cellspacing="3" width="50%" height="30%">
        <tr>
            <th>S.No.</th>
            <th>Subject Code</th>
            <th>Subject Name</th>
        </tr>
        <tr>
            <td>1.</td>
            <td>19A1414</td>
            <td>Fundamentals of Web Application Development(FWAD)</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>19A1301</td>
            <td>Python Programming(PP)</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>19EN101</td>
            <td>Communicative English(CE)</td>
        </tr>
        </table>   


```
# OUTPUT
<img width="1916" height="1019" alt="Screenshot 2025-11-27 232635" src="https://github.com/user-attachments/assets/d97e1d09-611f-4c94-bf6e-f12be3e7c10d" />


# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
