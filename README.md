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
```

## 2. Install Dependencies
Install the required dependencies by running:


```npm install```
This will install all the necessary packages listed in the package.json file.


## 3. Set Up Environment Variables

Create a .env file in the root directory of the project.
Add the following environment variables to the .env file:
env
```
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.eqxjz.mongodb.net/myDatabase?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret_key
PORT=3007
```
## 4.Explanation of Each Variable:
### MONGO_URI: 
-The connection string for your MongoDB Atlas database.
-Replace <username> and <password> with your MongoDB Atlas credentials.
-Make sure to use your actual MongoDB Atlas cluster URL.
### JWT_SECRET:
-A secure, random key for signing JSON Web Tokens (JWTs). You can use a random generator tool for extra security.
### PORT: 
-The port where your application will run. Default is 3007, but you can set this to any available port.


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

## 5. MongoDB Atlas Configuration

Ensure your MongoDB Atlas cluster is properly set up by following these steps:

1. **Create an Account**  
   Visit [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) and sign up for an account.

2. **Create a Project and Cluster**  
   - Once logged in, create a new project in MongoDB Atlas.  
   - Set up a cluster by choosing the free tier or any other plan as per your requirements.

3. **Whitelist Your IP Address**  
   - Go to the **"Network Access"** tab.  
   - Click **"Add IP Address"** and choose **"Allow Access from Anywhere"** (or add your specific IP).  

   > **Note:** For enhanced security, avoid using "Allow Access from Anywhere" in production. Instead, specify trusted IPs only.

4. **Create a Database User**  
   - Go to the **"Database Access"** section.  
   - Click **"Add New Database User"** and provide a username and password.  
   - Assign **"Read and Write"** permissions to this user.

5. **Obtain the Connection String**  
   - Go to your cluster's dashboard.  
   - Click **"Connect"** and select **"Connect Your Application"**.  
   - Copy the provided connection string.  

   Replace `<username>` and `<password>` in the string with your database user credentials.

6. **Add the Connection String to Your .env File**  
   Open your `.env` file and paste the connection string as shown below:


## 6. Troubleshooting
### Common Issues:
### 1. Database Connection Failed
Check if the MONGO_URI in .env is correct.
Ensure your MongoDB instance is running (locally or on Atlas).
### 2. Port Already in Use
If the default port 3007 is occupied, update the PORT value in .env to an unused port (e.g., PORT=3008).


