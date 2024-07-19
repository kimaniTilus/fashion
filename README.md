#README 
Obituary Management Platform

Overview

The Obituary Management Platform is a web application designed to facilitate the submission, management, and display of obituaries. This platform provides an easy-to-use interface for users to submit obituaries and view them. Additionally, it includes features for SEO and Social Media Optimization to enhance visibility and engagement.

Features

Obituary Submission: Users can submit obituaries through a user-friendly HTML form.
Database Management: Stores obituary data in a MySQL database.
Data Retrieval and Display: Retrieves and displays obituaries in a paginated and styled HTML table.
SEO Optimization: Dynamically generates meta tags, uses semantic HTML, and includes structured data for better search engine visibility.
Social Media Integration: Implements Open Graph tags and social media sharing buttons for better social media sharing previews.
Canonical Tags: Uses canonical tags to avoid duplicate content issues.
XML Sitemap: Generates and submits an XML sitemap to search engines for better indexing.
Technologies Used
Framework: Django
Database: MySQL
Frontend: HTML, CSS, JavaScript
SEO and Social Media: Meta tags, Open Graph tags, schema.org structured data
Setup Instructions
Environment Setup
Set up a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install dependencies:

pip install django mysqlclient
Configure the database: Update settings.py with your MySQL database settings:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'obituary_platform',
        'USER': 'your_db_user',
        'PASSWORD': 'your_db_password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
Run migrations:

python manage.py migrate
Create a superuser:

python manage.py createsuperuser
Start the development server:

python manage.py runserver
Usage
Submit Obituaries: Navigate to http://127.0.0.1:8000/submit_obituary/ to submit obituaries.
View Obituaries: Navigate to http://127.0.0.1:8000/view_obituaries/ to view obituaries.
SEO and Social Media Features
Dynamic Meta Tags: Meta tags for title, description, and keywords are dynamically generated based on the obituary content.
Semantic HTML and Structured Data: Uses semantic HTML tags and schema.org structured data to improve search engine visibility.
Open Graph Tags: Optimizes obituaries for social media sharing by adding Open Graph tags.
Social Media Sharing Buttons: Includes buttons for sharing obituaries on Facebook and Twitter.
Canonical Tags: Uses canonical tags to prevent duplicate content issues.
XML Sitemap: Generates an XML sitemap to help search engines index the site better.
Contributions
Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

