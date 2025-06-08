This Healthcare Chatbot project is a web-based application designed to assist users with healthcare-related queries through an interactive chatbot interface. Built with Django and integrated with machine learning libraries, the system leverages natural language processing and speech synthesis (using pyttsx3) to provide real-time, personalized healthcare advice. The backend uses a MySQL database managed via XAMPP for data storage and retrieval. This solution aims to improve accessibility to healthcare information and support users in managing their health efficiently.


Healthcare Chatbot Setup Instructions
Step 1: Setup Virtual Environment & Install Dependencies
Navigate to the code folder:
cd code

Create a virtual environment:
python -m venv venv

Activate the virtual environment:
On Windows: venv\Scripts\activate

Upgrade setuptools and wheel:
pip install --upgrade setuptools wheel

Install required Python packages:
pip install django==4.1
pip install pandas
pip install pyttsx3
pip install scikit-learn
pip install -r requirements.txt

Step 2: Setup Database with XAMPP
Open XAMPP Control Panel and start:
Apache
MySQL

Open your browser and visit:
http://localhost/phpmyadmin

Create a new database named:
healthcare

Step 3: Optional Configuration
To add a root password, edit the file:
C:\xampp1\phpMyAdmin\config.inc.php
Add or modify this line:
$cfg['Servers'][$i]['password'] = '7878';

To change the MySQL port, update your settings.py file:
'PORT': '3307'

Step 4: Run Migrations & Create Superuser
In terminal, run migrations:
python manage.py migrate

To create a superuser for admin access:
python manage.py createsuperuser

Step 5: Access the Website
Once the chatbot service is running, visit:
http://localhost:8000/
