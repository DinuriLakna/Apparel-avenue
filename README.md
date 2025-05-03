# Apparel-Avenue

## Project Overview
Apparel Avenue is an e-commerce platform developed as a group project for the Information Technology Project module in the 2nd year, 2nd semester. The platform facilitates online shopping for apparel, offering a seamless experience for customers, customer care managers, inventory managers, and finance managers. This project encompasses various functionalities, including product browsing, order management, and customer feedback systems.

# Customer Feedback and Complaint Management System
The Customer Feedback and Complaint Management System is a key component of Apparel Avenue, designed to handle customer feedback and complaints efficiently. Below is an overview of the system's features and workflows:
Features

CRUD Operations for Customers:

Create: Customers can submit feedback or complaints after receiving their orders.
Read: Customers can view their submitted feedback or complaints.
Delete: Customers can delete their feedback or complaints if needed.


Complaint Handling:

If a customer submits a complaint, they can request a refund or return for issues such as:
Incorrect order received.
Damaged product.


Customers provide details of the issue, which are logged for review.


Customer Care Manager Interface:

A dedicated interface for the customer care manager to review refund or return requests.
The manager evaluates the validity of the complaint:
Approve: If the reason is valid (e.g., damaged product or incorrect order), the request is approved.
Reject: If the reason is invalid, the request is rejected, and the customer is notified.


Return and Refund Workflow:

Upon receiving a returned order, the customer care manager performs the following:
Notifies the Finance Manager: Informs about the financial loss due to the damaged order.
Notifies the Inventory Manager: Requests an update to the inventory if the return is due to an incorrect size.


System Workflow

Customer Submission:

The customer submits feedback or a complaint via the customer interface after receiving an order.
For complaints, they specify if they seek a refund or return and provide supporting details.


Customer Care Review:

The customer care manager accesses the separate interface to review complaints.
The manager approves or rejects the refund/return request based on the provided evidence.


Post-Return Actions:

If a return is processed, the customer care manager notifies:
The Finance Manager to account for the loss.
The Inventory Manager to update stock (e.g., for incorrect size returns).


# Installation and Setup
To run the Apparel Avenue project locally, follow these steps:
Prerequisites

Node.js (for frontend and backend)
MySQL (for database)
Git (for cloning the repository)

Steps

Clone the Repository:
git clone https://github.com/DinuriLakna/Apparel-avenue.git
cd Apparel-avenue


Install Dependencies:

For the backend:cd backend
npm install

For the frontend:cd frontend
npm install


Database Setup:

Create a MySQL database named apparel_avenue.
Import the database schema from backend/database/schema.sql:mysql -u <username> -p apparel_avenue < backend/database/schema.sql


Run the Application:

Start the backend server:cd backend
npm start


Start the frontend:cd frontend
npm start


Access the Application:

Open your browser and navigate to http://localhost:3000 for the customer interface.
The customer care manager interface is accessible at http://localhost:3000/admin (credentials required).



# Technologies Used

Frontend: React.js, Tailwind CSS
Backend: Node.js, Express.js
Database: MySQL
Authentication: JSON Web Tokens (JWT)
Other Tools: Git, npm

# Team Contributions

Customer Feedback and Complaint Management System: Implemented by Lakna Dassanayake.
Developed CRUD operations for customer feedback and complaints.
Built the refund and return request system.
Designed the customer care manager interface for request reviews.
Integrated notifications for finance and inventory managers.
Other modules (e.g., product browsing, order management) were implemented by other team members.

# Future Enhancements

Add real-time notifications for customers on complaint status updates.
Implement an AI-based system to pre-evaluate complaint validity.
Enhance the customer care interface with analytics for complaint trends.
