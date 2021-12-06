# INSTALLATION

1. FORK THE REPO
2. CLONE THE REPO
3. INSTALL DEPANDANCY OF THE PROJECT

- npm i express ejs express-session express-validator bcryptjs mysql2

4. SET UP MYSQL DATABASE
   1. CREAT THE TABLE - ```
      CREATE TABLE users (
      id int(10) unsigned NOT NULL AUTO_INCREMENT,
      name varchar(50) COLLATE utf8mb4_unicode_ci NOT NULL,
      email varchar(50) COLLATE utf8mb4_unicode_ci NOT NULL,
      password varchar(255) COLLATE utf8mb4_unicode_ci NOT NULL,
      PRIMARY KEY (id),
      UNIQUE KEY email (email)
      ) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;
      }

```
        2. SET UP DATABASE FOR PROJECT
        (IN dbconnect.js file below set up)
       - const mysql = require('mysql2');

const dbConnection = mysql.createPool({
    host: 'localhost',
    user: 'root',
    password: '',
    database: 'nodejs_login'
});

module.exports = dbConnection.promise();

5. RUN THE PROJECT
   - Node index.js



# RITU- Period Tracker

#### TODO
* [ ] service worker - work offline
* [ ] background syncronisation
* [ ] use google calendar as backend server
* [ ] show error if erroring when add/update/delete
* [ ] when during event, different homescreen
* [ ] implement edit entry UI functionality
```
