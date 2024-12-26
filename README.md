# zidio_dev_blueprint_task_app

# Cloud-Based Kanban Board

This web application is designed to streamline task management for individuals and teams using the Kanban methodology. Built with the MERN stack (MongoDB, Express.js, React, and Node.js), this platform offers a visual interface for organizing tasks into stages (to-do, in-progress, done) and facilitates efficient task management.

**Why/Problem**

Traditional task management methods often lack the visual clarity to effectively prioritize and track tasks. The Cloud-Based Kanban Board addresses this challenge by providing a drag-and-drop interface for intuitive task organization and progress visualization.

**Features**

* **Task Management:**
    * Create, edit, and delete tasks.
    * Assign tasks to users.
    * Set deadlines for tasks.
* **Kanban Board:**
    * Drag and drop tasks between stages (to-do, in-progress, done).
    * Visualize workflow progress.
* **User Management:**
    * User registration and login.
    * Role-based access control (optional).
* **Collaboration:**
    * Add comments and discussions to tasks (optional).

**Technologies**

* **Frontend:**
    * React (Vite)
    * Redux Toolkit for state management
    * React Beautiful DnD for drag-and-drop functionality
    * Material UI for a modern and consistent design

* **Backend:**
    * Node.js with Express.js
    * Mongoose for interacting with the MongoDB database

* **Database:**
    * MongoDB for storing task data and user information

**Setup Instructions**

1. **Server Setup**
    * Create a `.env` file in the server directory to store environment variables like MongoDB connection URI, JWT secret, and port number.
         - MONGODB_URI = `your MongoDB URL`
         - JWT_SECRET = `any secret key - must be secured`
         - PORT = `8800` or any port number
         - NODE_ENV = `development`
    * Set up a MongoDB database and configure the connection URL in the `.env` file.
       - Create an Account
          - Log in to your MongoDB Atlas account.
          - Create a New Cluster
          - Choose a Cloud Provider and Region
          - Configure Cluster Settings
          - Create Cluster
          - Wait for Cluster to Deploy
          - Create Database User
          - Set Up IP Whitelist
          - Connect to Cluster
          - Configure Your Application
          - Test the Connection
    * Install dependencies using `npm install`.
    * Start the server using `npm start`.
  
1. Open the project in any editor of choice.
2. Navigate into the server directory `cd server`.
3. Run `npm i` or `npm install` to install the packages.
4. Run `npm start` to start the server.

2. **Client Setup**
    * Create a `.env` file in the client directory to store the base URL of the server and any other necessary environment variables.
         - VITE_APP_BASE_URL = `http://localhost:8800` #Note: Change the port 8800 to your port number.
         - VITE_APP_FIREBASE_API_KEY = `Firebase api key`
    * Install dependencies using `npm install`.
    * Start the client application using `npm start`.
  
1. Navigate into the client directory `cd client`.
2. Run `npm i` or `npm install` to install the packages.
3. Run `npm start` to run the app on `http://localhost:3000`.
4. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

**Deployment**

* Deploy the server-side application to a cloud platform like Heroku or AWS.
* Deploy the client-side application to a static hosting platform like Netlify or Vercel.

**Further Enhancements**

* Integrate real-time updates using web sockets or a pub/sub messaging system.
* Implement user notifications for task updates and mentions.
* Add analytics to track user activity and project progress.

This project provides a solid foundation for a cloud-based Kanban board application. You can customize and extend it with additional features to suit your specific needs and showcase your technical skills during your internship.

Remember to replace placeholders like `your MongoDB URL` and `any secret key` with your actual values. Also note that some features like real-time updates and user notifications are optional and can be added for complexity.
