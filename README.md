Ethereum Deposit Tracker

Project Overview

The Ethereum Deposit Tracker is an application that monitors and records ETH deposits made to the Beacon Deposit Contract on the Ethereum blockchain. It interfaces with an Ethereum node via Infura or Alchemy to track and log deposits in real-time.

Features

Real-Time Monitoring: Tracks ETH deposits to the Beacon Deposit Contract.
Detailed Logging: Captures deposit details including block number, timestamp, transaction hash, and more.
Error Handling: Includes robust mechanisms for error handling and logging.
Optional Notifications: Provides optional Telegram notifications for new deposits.
Extendable: Can be enhanced with visualization tools like Grafana or integrated with a database.
Bonus: Dockerized for simplified deployment.
Prerequisites

Before getting started, ensure you have the following:

Node.js (version 12.x or higher)
npm (Node Package Manager)
Access to an Ethereum RPC provider such as Infura or Alchemy
(Optional) A Telegram bot for notifications
(Optional) Docker for containerization
Backend Setup (Node.js + ethers.js)

Clone the Repository or Set Up a New Project Directory:
sh
Copy code
git clone https://github.com/parthhiv-pathakk/Final_Luganodes.git
cd Final_Luganodes
Install Backend Dependencies:
sh
Copy code
npm install


Running the Project

Backend Setup (Node.js + ethers.js)
Start the Backend:
In the eth-deposit-tracker directory, run the following command to launch the backend server:

sh
Copy code
node server.js
This will start the backend server on port 3001. The backend will monitor Ethereum blocks and log any deposits made to the Beacon Deposit Contract.
Frontend Setup (React.js)
Navigate to the Frontend Directory:
Move to the eth-deposit-frontend directory:

sh
Copy code
cd ../eth-deposit-frontend
Install Frontend Dependencies:
Install the necessary dependencies for the frontend:

sh
Copy code
npm install
Run the Frontend:
Start the frontend development server with:

sh
Copy code
npm start
The frontend will be accessible at http://localhost:3001. It fetches deposit data from the backend at http://localhost:3001/deposits and displays it in a table.
Usage Instructions

Starting the Project
Start the Backend:
Open a terminal, navigate to the eth-deposit-tracker directory, and execute:

sh
Copy code
node server.js
This command will:

Track Ethereum blocks in real-time.
Log detected deposits to deposits.log.
Serve deposit data at http://localhost:3001/deposits.
Start the Frontend:
Open another terminal window, navigate to the eth-deposit-frontend directory, and run:

sh
Copy code
npm start
The frontend will start and be available at http://localhost:3001, displaying deposit information fetched from the backend.
