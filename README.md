# RESTFul Flutter Recipe Practice Project

This project is supposed to be a practice project for a RESTFul Flutter application using a Django Backend. The app is supposed to be extremely simple with no authentication logic. The app is only supposed to display a list of recipes from a database and display its information. I am planning to first create the base app after which I will work on making the UI better along with responsiveness and adaptiveness.


<h3>
Python environment packages
</h3>
<br>

pip install Django
<br>
pip install djangorestframework
<br>
pip install django-cors-headers
<br>
pip install python-dotenv
<br>


<h3>
Variables excluded from settings.py
</h3>

Variables SECRET_KEY, DEBUG and ALLOWED_HOSTS have been omitted. Please use your own when you create the project and remove the following code (line 15 to 23):

from dotenv import load_dotenv
import os
load_dotenv(os.path.join(os.path.dirname(__file__), '../.env'))
SECRET_KEY = os.getenv('SECRET_KEY')  # Uses value from .env
DEBUG = os.getenv('DEBUG') == 'True'  # Converts string to boolean
ALLOWED_HOSTS = os.getenv('ALLOWED_HOSTS').split(',')