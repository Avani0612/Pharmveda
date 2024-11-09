
Welcome to my React and Node tutorial, where we'll construct a dynamic food delivery app using the MERN stack (MongoDB, ExpressJS, React, and Node.JS). This tutorial guides you through each step, from setting up MongoDB as our database to crafting user interfaces with React and implementing server-side logic with Node.JS and ExpressJS. Our aim is to provide a comprehensive understanding of how these technologies come together to create a feature-rich food delivery app named "Foodie."
## You Will Learn

- HTML5 and CSS3: Semantic Elements, CSS Grid, Flexbox
- React: Components, Props, Events, Hooks, Router, Axios
- Context API: Store, Reducers, Actions
- Node & Express: Web API, Body Parser, File Upload, JWT
- MongoDB: Mongoose, Aggregation
- Development: ESLint, Babel, Git, Github,  
- Deployment: Heroku

## Run Locally

### 1. Clone repo

```
$ git clone git@github.com:basir/mern-foodie.git
$ cd mern-foodie
```

### 2. Create .env File

- duplicate .env.example in backend folder and rename it to .env

### 3. Setup MongoDB

- Local MongoDB
  - Install it from [here](https://www.mongodb.com/try/download/community)
  - In .env file update MONGODB_URI=mongodb://localhost/foodie
- OR Atlas Cloud MongoDB
  - Create database at [https://cloud.mongodb.com](https://cloud.mongodb.com)
  - In .env file update MONGODB_URI=mongodb+srv://your-db-connection

### 4. Run Backend

```
$ cd backend
$ npm install
$ npm start
```

### 5. Run Frontend

```
# open new terminal
$ cd frontend
$ npm install
$ npm start
```

### 6. Seed Users and Products

- Run this on browser: http://localhost:5000/api/seed
- It returns admin email and password and 6 sample products

### 7. Admin Login

- Run http://localhost:3000/signin
- Enter admin email and password and click signin


