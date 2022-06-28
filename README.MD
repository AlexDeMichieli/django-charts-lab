## Django - Charts lab

Step 1 - Getting Started 

- Create and enable a virtual environment

- install all the dependencies:

```
pip install -r requirements.txt
```

- Make migrations, migrate and add a superusers:

```
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
```
- Make sure that the server runs without issues:

```
python manage.py runserver
```

## Start from the home.html page

The `home.html` page includes code that is responsible for updating the database with a new product via POST request through django-rest.

You will be provided with a form and a (almost fully written) JavaScript fetch function. You'll need to spend some time reading the function and understand where the input from the form should fit in the function itself.

You should use the console panel in the browser to debug possible errors and visit the admin page (http://127.0.0.1:8000/admin/) to verify if a new proudct appears after each call.

## Step 2 - the chart.html page

Once you are able to post a prouct correctly, you'll move the the chart.html page. This page is blank. You'll need to implement a chart of your choice using the [charts.js](https://www.chartjs.org/) library.

In order to make this work, you'll need to:

1. make a GET request to the following endpoint: 

http://127.0.0.1:8000/api/products/

2. Grab the data and ingest it in the chart

