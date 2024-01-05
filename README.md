# Simple login with Nodejs

Objective of this article is to create a basic login system, whose back-end will be written in Node.js using Express framework and it will render HTML pages for registering users and allowing them to login. But we won’t be dealing with sessions in this article.

Typically, this type of project needs a database to store the credentials. But, we won’t use that as well, as this project is only to give an overview of login system. So, we’ll be using arrays to store the user credentials. Once, we shut down the server, all the credentials will be deleted.

First:

```
npm init
```

Second:

```
npm install express bcrypt body-parser --save
```

_Express_ : is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. With the help of express, APIs can be build very easily and quickly.

_Bcrypt_ : is a library that helps us to hash passwords.

_Body-parser_ : is required to handle HTTP POST request in Express.js. It extracts the entire body portion of an incoming request stream and exposes it on req.body.

Response example of register:

```
User list [
  {
    id: 1704459048095,
    username: 'joão',
    email: 'seuemail@email',
    password: '$2b$10$EB8oAX1mv8HH2sCY6XO2uOysjcakg/rYqjXOJADC8Z0k88tUmZPVa'
  }
]
```
