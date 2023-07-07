# Sales Prediction Analysis

## Tech Stacks Used:

- Angular.js
- Python (Flask)
- MongoDB
- Machine learning model (SARIMAX Model)
- Email.js 




## :point_down:Steps to initialize the project:

- Clone the repository

```
$ git clone https://github.com/Vigneshwar-B/sales-forcasting.git
```

- Redirect to the cloned repo directory

- Open up the terminal and redirect to client directory.

- Install the dependencies

```
npm install
```

- create the mongoDB account in the mongoDB atlas and create the cluster

- Note: A guide to create the mongoDB account and mongoDB URL
  https://www.youtube.com/watch?v=oVHQXwkdS6w


- click on connect and select connect your application.

- select python as Driver and select version as per the version that you have installed in your PC and get the MONGO DB url from it

- Then create the database user by clicking the database access from the mongoDB atlas menu and click on `Add New Database User`. Then provide the username and password and set the built-in role as `read and write to any database` and click on Add user.

- Replace the DB user name and password in the MongoDB URL.

- Paste the MongoDB URL in app.py file `/server/app.py`

![image](https://user-images.githubusercontent.com/84177086/211177985-2f65f5ac-bf7a-436a-9470-e381841e6fdc.png)

- To create the database, click the database from the mongoDB atlas menu. Then click `Browse Collections` and click `Create Database`

- Note: The database should be named as `SalesPrediction` and  the collection should be named as `account` .

- Create the Secret key typing the following command in the terminal.

```
python -c 'import os; print(os.urandom(24))';
```

- Secret key will be generated and paste it in app.py file `/server/app.py`

![image](https://user-images.githubusercontent.com/84177086/211178109-65428e1a-c945-4033-b28f-87ea1ffe7f58.png)

- Use email.js for sending the contact form data to your email inbox

- Create the email.js account in `https://www.emailjs.com/` and paste the service id, template id and user id in `/client/src/app/components/contact-us/contact-us.component.ts`

![image](https://user-images.githubusercontent.com/84177086/211178227-ee5ff76c-3bd4-4408-af31-bb505fd8a228.png)

- A guide to Email.js

  https://www.youtube.com/watch?v=dgcYOm8n8ME





- For starting the client, type the following in the command prompt

```
cd client 
```
```
ng serve -o
```

- For starting the server, type the following in the new command prompt

```
cd server
```
```
flask --app app --debug run
```

- Note: This Application will be worked only for the following single dataset.

[sales_data_sample.csv](https://github.com/Vigneshwar-B/salesforcasting/blob/a566b13c72e7d550ed186dd813c06c9f1197ea01/sales_data_sample.csv)


