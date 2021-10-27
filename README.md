# E-commerce Back End

# Purpose
This application serves as the backend of an e-commerce site, which uses a functional Express.js API and uses Sequelize to interact with a MySQL database.

When the user adds their database name, MySQL username, and MySQL password to an environmental variable file, the user is able to connect to a database using Sequelize. When entering schema and seed commands, a development database is created and is seeded with test data. When the application is invoked, the server is started and Sequelize models are synced to the MySQL database, with API GET routes for categories, products, and tags display a formatted JSON using Insomnia Core or Postman. When testing API POST, PUT, and DELETE routes in Insomnia Core, users can create, update, and delete data in the database.

MySQL2 and Sequelize packages connect the Express.js API to a MySQL database. The dotenv package uses environmental variables to store sensitive data, such as the user's MySQL username, password, and database name. On server start, the application syncs Sequelize models of Category, Product, Tag, and ProductTag to a MySQL database and includes associations between these models.

The associations are as follows:

* Product belongs to Category, as a category can have multiple products but a product can only belong to one category.

* Category has many Product models.

* Product belongs to many Tag models. Using the ProductTag through model, allow products to have multiple tags and tags to have many products.

* Tag belongs to many Product models.

In the future, this project may be refactored for improved efficiency and readability.

# Built With
* JavaScript
* HTML
* CSS
* Express.js
* MySQL2 https://www.npmjs.com/package/mysql2
* Sequelize https://www.npmjs.com/package/sequelize
* dotenv package

# Usage
Clone the repository, navigate to the project folder in your CLI and use the ```npm run seed``` to seed data to the database and test CRUD routes.

# Questions
For additional questions and information, please go to github.com/maxaeon/
or reach out via email at maparks@ucdavis.edu.
# License
MIT License

Copyright (c) [2021] 

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


