Sales Prediction Analysis
Tech Stacks Used:
Angular.js
Python (Flask)
MongoDB
Machine learning model (SARIMAX Model)
Email.js
Demo Video 👇
 Sales.Prediction.Analysis.mp4 
👇Steps to initialize the project:
Clone the repository
$ git clone https://github.com/anjupriya-v/sales-prediction-analysis.git
Redirect to the cloned repo directory

Open up the terminal and redirect to client directory.

Install the dependencies

npm install
create the mongoDB account in the mongoDB atlas and create the cluster

Note: A guide to create the mongoDB account and mongoDB URL https://www.youtube.com/watch?v=oVHQXwkdS6w

click on connect and select connect your application.

select python as Driver and select version as per the version that you have installed in your PC and get the MONGO DB url from it

Then create the database user by clicking the database access from the mongoDB atlas menu and click on Add New Database User. Then provide the username and password and set the built-in role as read and write to any database and click on Add user.

Replace the DB user name and password in the MongoDB URL.

Paste the MongoDB URL in app.py file /server/app.py

image

To create the database, click the database from the mongoDB atlas menu. Then click Browse Collections and click Create Database

Note: The database should be named as SalesPrediction and the collection should be named as account .

Create the Secret key typing the following command in the terminal.

python -c 'import os; print(os.urandom(24))';
Secret key will be generated and paste it in app.py file /server/app.py
image

Use email.js for sending the contact form data to your email inbox

Create the email.js account in https://www.emailjs.com/ and paste the service id, template id and user id in /client/src/app/components/contact-us/contact-us.component.ts

image

A guide to Email.js

https://www.youtube.com/watch?v=dgcYOm8n8ME

Email.js Content template screenshot 👇
image

Email.js Auto reply template screenshot 👇
image

For starting the client, type the following in the command prompt
cd client 
ng serve -o
For starting the server, type the following in the new command prompt
cd server
flask --app app --debug run
Note: This Application will be worked only for the following single dataset.
