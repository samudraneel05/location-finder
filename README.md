# Latitude-Longitude-To-Address-Converter

## Video Demo:

[![Location Finder by Samudraneel Sarkar](https://img.youtube.com/vi/2fnCCudjtEw/0.jpg)](https://www.youtube.com/watch?v=2fnCCudjtEw)

Click on the image above or this URL - https://youtu.be/2fnCCudjtEw

## Description:

A web application that accepts Latitude and Longitude co-ordinates and displays the corresponding address. Libraries and modules used include geopy, css from w3schools and bootstrap, and CSV file information is handled in the project.

The app has three primary directories, **LatLong, templates and app** . Apart from that, it also has two files called **project.py** and **test_project.py**, which are responsible for handling all of the django setup-checkup syntax and error testing respectively. It also has a database **db.sqlite3** made in SQL to handle coordinates.

### LatLong:
The LatLong folder consists of three files **settings.py**, **urls.py** and **wsgi.py**.

settings.py handles all of the django settings including installed applications, middleware and route URL configuration. It also notes the database and password validators. The file urls.py imports admin from the django contrib library and sets the url path, whereas wsgi.py sets the default django settings module and imports from django core wsgi application.

### Templates:
The templates folder has the **index.html** file and the CSS style sheet **style.css** which is referenced throughout.

The index page consists of a form that allows the user to enter latitude and longitude that is submitted through the help of button. It then outputs a street address after the back end does all the processing. The style.css adds styling guides for the navigation bar, the HTML body and specific tags.

### App:
The app folder consists of **admin.py**, **apps.py**, **latLongToAddressConverter.py**, **latLongToAddressConverterFromCSV.py**, **tests.py**, **urls.py** and **views.py**.

admin.py allows one to register one's models, whereas apps.py sets the name of the django web applicsation to app. latLongToAddressConverter.py and latLongToAddressConverterFromCSV.py have the code for converting the users input in forms of decimals or comma separated values to street address or location information. The file tests.py is for internal error checking and urls.py handles the url changes after the information of street address appears on screen. views.py handles the html requests and request methods through django and python code.

## Usage:

Run the following on your terminal - `python3 project.py runserver`
