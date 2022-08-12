I wanted to create an application to allow users utilize a blog application to defend their champions and heroes. The users will be able to create blog posts, access all blog posts, edit their blog posts by updating or deleting the posts, and comment on any blog posts. The users will be required to sign in to perform all of the functions listed besides accessing all of the blog posts. At the end of the day, the users may choose to log out of the blog for security.
Installation

If you would like to access the app via localhost, you will first need to install the node modules after cloning this repository with the following code:

npm i
After that, the node modules will be installed.

Before launching the application via localhost, you will need to edit and add to the ".env.EXAMPLE" file with the following steps:

Change the ".env.EXAMPLE" file name to ".env"
Fill out the ".env" file by adding your MYSQL username, password, and your session key. Please find an example below:
DB_USER="temp username"
DB_PASSWORD="temp password"
DB_NAME=marvel_battlefield_db
SESSION_SECRET="your session secret key"
The database name will be left as it is as you will be accessing the application's database. If you would like to change the database name, the database names in the .env.EXAMPLE and schema.sql files will need to be changed as well.

Next, you will need to create the database by running the following code in MYSQL from your main branch, which will load the schema.sql:

source db/schema.sql;
Then, you will need to run the following code on your main branch in your terminal or Git Bash:

npm run seed
Finally, you run the following code to start the localhost or via nodemon respectively:

npm start
or

npm run watch
With all of the steps above, you can visit http://localhost:3001 to access the application.

# Hero Deployment link:
https://dashboard.heroku.com/apps/mvcproject2

# Github Deploment link:
https://github.com/mshehroz237/mvc-project

# Pictures
<img width="1440" alt="Screen Shot 2022-08-11 at 10 31 47 PM" src="https://user-images.githubusercontent.com/97645096/184274279-22d41536-4eba-4dc6-af6a-2d67cb8e00ac.png">
<img width="1440" alt="Screen Shot 2022-08-11 at 10 31 38 PM" src="https://user-images.githubusercontent.com/97645096/184274284-0f9057a9-acd4-4654-b80d-37bfacb96e72.png">
<img width="1440" alt="Screen Shot 2022-08-11 at 10 31 11 PM" src="https://user-images.githubusercontent.com/97645096/184274287-031d37e3-86db-41d4-afe1-0b68df872fa2.png">
