# E_Commerce

## Project Setup Guide

This guide will walk you through the process of setting up and running the project on your local machine.

---

## Prerequisites

Before starting, ensure you have the following installed:

- [Node.js](https://nodejs.org/en/download/) (v12.x or higher)
- [MongoDB](https://www.mongodb.com/try/download/community) (or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for a cloud database)
- [npm](https://www.npmjs.com/get-npm) (comes with Node.js installation)
- A code editor like [VS Code](https://code.visualstudio.com/)

---

## 1. Clone the Repository

To clone the repository, run:

```bash
git clone https://github.com/CVJaswanthiReddy/E_Commerce.git
cd E_Commerce

## 2.Install Dependencies

Install the required dependencies by running:

```bash
npm install
```
This will install all the necessary packages listed in the package.json file.


Sure! Here's the updated README.md with the correct GitHub repository link in the Clone the Repository section:

markdown
Copy code
# E-Commerce

## Project Setup Guide

This guide will walk you through the process of setting up and running the project on your local machine.

---

## Prerequisites

Before starting, ensure you have the following installed:

- [Node.js](https://nodejs.org/en/download/) (v12.x or higher)
- [MongoDB](https://www.mongodb.com/try/download/community) (or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for a cloud database)
- [npm](https://www.npmjs.com/get-npm) (comes with Node.js installation)
- A code editor like [VS Code](https://code.visualstudio.com/)

---

## 1. Clone the Repository

To clone the repository, run:

```bash
git clone https://github.com/CVJaswanthiReddy/E_Commerce.git
cd E_Commerce
2. Install Dependencies
Install the required dependencies by running:


```npm install```
This will install all the necessary packages listed in the package.json file.

##3. Set Up Environment Variables

Create a .env file in the root directory of the project.
Add the following environment variables to the .env file:
env
```
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.eqxjz.mongodb.net/myDatabase?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret_key
PORT=3007
```
## Explanation of Each Variable:
### MONGO_URI: The connection string for your MongoDB database.

### For MongoDB Atlas: Replace <username> and <password> with your credentials.
### For local MongoDB: Use mongodb://localhost:27017/myDatabase.
### JWT_SECRET: A secure, random key for signing JSON Web Tokens (JWTs). You can use a random generator tool for extra security.

### PORT: The port where your application will run. Default is 3007, but you can set this to any available port.

## 4. Start the Server
To run the project, execute:

```
npm start
```
For development mode with auto-reload, use:

```
npm run dev
```
By default, the server will be accessible at:

```
http://localhost:3007
```
If the PORT is changed, replace 3007 with your specified port.

## 5. MongoDB Configuration (Optional)
### If using MongoDB Atlas:

Ensure your cluster is properly set up.
Whitelist your current IP address in the Atlas dashboard.
Refer to the MongoDB Atlas Documentation for further details.


Sure! Here's the updated README.md with the correct GitHub repository link in the Clone the Repository section:

markdown
Copy code
# E-Commerce

## Project Setup Guide

This guide will walk you through the process of setting up and running the project on your local machine.

---

## Prerequisites

Before starting, ensure you have the following installed:

- [Node.js](https://nodejs.org/en/download/) (v12.x or higher)
- [MongoDB](https://www.mongodb.com/try/download/community) (or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for a cloud database)
- [npm](https://www.npmjs.com/get-npm) (comes with Node.js installation)
- A code editor like [VS Code](https://code.visualstudio.com/)

---

## 1. Clone the Repository

To clone the repository, run:

```bash
git clone https://github.com/CVJaswanthiReddy/E_Commerce.git
cd E_Commerce
2. Install Dependencies
Install the required dependencies by running:

bash
Copy code
npm install
This will install all the necessary packages listed in the package.json file.

3. Set Up Environment Variables
Create a .env file in the root directory of the project.
Add the following environment variables to the .env file:
env
Copy code
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.eqxjz.mongodb.net/myDatabase?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret_key
PORT=3007
Explanation of Each Variable:
MONGO_URI: The connection string for your MongoDB database.

For MongoDB Atlas: Replace <username> and <password> with your credentials.
For local MongoDB: Use mongodb://localhost:27017/myDatabase.
JWT_SECRET: A secure, random key for signing JSON Web Tokens (JWTs). You can use a random generator tool for extra security.

PORT: The port where your application will run. Default is 3007, but you can set this to any available port.

4. Start the Server
To run the project, execute:

bash
Copy code
npm start
For development mode with auto-reload, use:

bash
Copy code
npm run dev
By default, the server will be accessible at:

arduino
Copy code
http://localhost:3007
If the PORT is changed, replace 3007 with your specified port.

5. MongoDB Configuration (Optional)
If using MongoDB Atlas:

Ensure your cluster is properly set up.
Whitelist your current IP address in the Atlas dashboard.
Refer to the MongoDB Atlas Documentation for further details.

## 6. Troubleshooting
### Common Issues:
### 1. Database Connection Failed
Check if the MONGO_URI in .env is correct.
Ensure your MongoDB instance is running (locally or on Atlas).
### 2. Port Already in Use
If the default port 3007 is occupied, update the PORT value in .env to an unused port (e.g., PORT=3008).


