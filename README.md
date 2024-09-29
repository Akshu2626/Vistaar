1. Project Overview
2. Technologies Used
3. Setup Instructions
    Backend Setup
    Frontend Setup
4. API Endpoints
5. Usage
6. Deployment


Project Overview : 

This project is a full-stack application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) that implements user authentication via JWT (JSON Web Token). The application allows users to sign up, log in, and access a protected home screen.


Technologies Used : 

Backend: Node.js, Express.js, MongoDB (with Mongoose), JWT for authentication
Frontend: React.js (with Vite), React Router for navigation
Others: dotenv for environment variables, cors for cross-origin resource sharing


Backend Setup : 
              git clone <repository-url>  
              cd <repository-name> 
              npm i  
              create .env file 
              ```PORT=4040
                MONGO_URI=mongodb+srv://Akshu26:12345@cluster0.opeazef.mongodb.net/vishtara?retryWrites=true&w=majority&appName=Cluster0
                JWT_SECRET=your_jwt_secret```
              run cmd : npm start or node server.js

Frontend Setup : 
                ```cd <repository-name>
                npm install
                npm run dev```

                
API Endpoints : 
            1.  URL: /api/signup
              Method: POST
             req.body= {
                    "username": "string",
                    "email": "string",
                    "password": "string"
                                        }
            2.  URL: /api/login
              Method: POST
              req.body={
                  "email": "string",
                    "password": "string"
                                        }
          3. URL: /api/home
                  Method: GET
                  header : Authorization: Bearer <your_jwt_token>

                  
Usage
1. Signup: Navigate to /signup to create a new account.
2. Login: Navigate to /login to log in with your credentials.
3. Home Page: Once logged in, you will be redirected to the home page, where you can see a welcome message and a logout button.
                                        
            

