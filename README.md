# Blockchain E-Voting System

## Overview

This project is a decentralized e-voting system built using a microservices architecture. It consists of three main components:

- **Frontend:** A React.js application using Vite for fast builds and TypeScript for type safety.
- **Backend:** A Node.js and Express.js service for user authentication.
- **Blockchain:** A smart contract-based service using Solidity and Web3.js, integrated with Sepolia test network.

## Directory Structure

- `frontend/`: Contains the React.js frontend application.
- `backend/`: Contains the Node.js backend service for user authentication.
- `blockchain/`: Contains the blockchain component with smart contracts.

## Setup and Run

### Prerequisites

- Node.js
- Docker and Docker Compose (optional, for containerized setup)
- MetaMask extension for browser
- Infura account

### 1. Clone the Repository

Clone the main repository:

```sh
git clone https://github.com/yourusername/blockchain-e-voting-system.git
cd blockchain-e-voting-system
```

### 2. Setup Each Component

#### Frontend

1. Navigate to the frontend directory:

   ```sh
   cd frontend
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Create a `.env` file (if required) and start the development server:

   ```sh
   npm run dev
   ```

4. Access the frontend at `http://localhost:3000`

#### Backend

1. Navigate to the backend directory:

   ```sh
   cd backend
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Create a `.env` file based on the provided `.env.example` template:

   ```plaintext
   PORT=4000
   ACCESS_TOKEN_SECRET=your_secret_key
   SUPERADMIN_EMAIL=superadmin@example.com
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=system
   DB_NAME=mydatabase
   DB_PORT=3307
   ```

4. Start the backend server:

   ```sh
   node start
   ```

5. Access the backend service at `http://localhost:4000`

#### Blockchain

1. Navigate to the blockchain directory:

   ```sh
   cd blockchain
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Create a `.env` file with the required configuration:

   ```plaintext
   INFURA_URL=https://sepolia.infura.io/v3/YOUR_INFURA_PROJECT_ID
   CONTRACT_ADDRESS=0x49Ff66b40F77c78e65aafC07451e218b91EE0f03
   YOUR_METAMASK_ADDRESS=YOUR_METAMASK_PUBLIC_ADDRESS
   PRIVATE_KEY=YOUR_METAMASK_PRIVATE_KEY
   ```

4. Start the blockchain service:

   ```sh
   node start
   ```

5. The blockchain service will run at `http://localhost:5173`

### 3. Running All Components with Docker (Optional)

If you prefer using Docker to manage the services, make sure you have Docker and Docker Compose installed. Then, use Docker Compose to start all services:

```sh
docker-compose up --build
```

### 4. Contributing

Please refer to the individual `README.md` files in the `frontend`, `backend`, and `blockchain` directories for specific contribution guidelines.

### License

This project is licensed under the MIT License.

## Additional Resources

- [MetaMask](https://metamask.io/)
- [Infura](https://infura.io/)
- [Soft UI Dashboard](https://www.creative-tim.com/product/soft-ui-dashboard) (Frontend Template)

### Summary

- **Overview:** Describes the overall project and its components.
- **Directory Structure:** Lists and explains the project structure.
- **Setup and Run:** Detailed setup instructions for each component (frontend, backend, blockchain).
- **Docker Setup:** Optional instructions for running the project with Docker.
- **Contributing:** Directs users to individual `README.md` files for contribution guidelines.
- **License:** States the license type.
- **Additional Resources:** Links to resources used in the project.

This main `README.md` provides comprehensive instructions for setting up and running the entire project, as well as details on individual components and optional Docker usage.
