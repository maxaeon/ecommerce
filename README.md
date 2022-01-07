# E-commerce Back End

# Purpose
This application serves as the backend of an e-commerce site, which uses a functional Express.js API and uses Sequelize to interact with a MySQL database.

When the user adds their database name, MySQL username, and MySQL password to an environmental variable file, the user is able to connect to a database using Sequelize. When entering schema and seed commands, a development database is created and is seeded with test data. When the application is invoked, the server is started and Sequelize models are synced to the MySQL database, with API GET routes for categories, products, and tags display a formatted JSON using Insomnia Core or Postman. When testing API POST, PUT, and DELETE routes in Insomnia Core, users can create, update, and delete data in the database.

MySQL2 and Sequelize packages connect the Express.js API to a MySQL database. The dotenv package uses environmental variables to store sensitive data, such as the user's MySQL username, password, and database name. On server start, the application syncs Sequelize models of Category, Product, Tag, and ProductTag to a MySQL database and includes associations between these models.

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

<img width="1133" alt="ecommerce4" src="https://user-images.githubusercontent.com/87254760/148495633-39d08bd4-0dae-4868-800b-2763a9339363.png">
<img width="1137" alt="ecommerce3" src="https://user-images.githubusercontent.com/87254760/148495636-d770a271-6c7f-4b61-b34e-0cdc1b8a7280.png">
<img width="1126" alt="ecommerce2" src="https://user-images.githubusercontent.com/87254760/148495637-685efe96-8df5-4e11-a798-7bfa5e9698f8.png">
<img width="1131" alt="ecommerce1" src="https://user-images.githubusercontent.com/87254760/148495639-89c85109-a20c-44be-8f75-0c414c15a197.png">
<img width="953" alt="ecommerce" src="https://user-images.githubusercontent.com/87254760/148495641-96c5532f-773f-4621-ba4c-5d28bd059745.png">


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


