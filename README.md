
# **TechDome Docker Compose Project**

This repository contains the Docker Compose configuration files for setting up and running the **TechDome** project, which includes a backend, frontend, and MongoDB database.

## **Overview**

The project includes:
- A **backend** service built with Node.js.
- A **frontend** service developed with React.js.
- A **MongoDB** database for storing application data.

The application is containerized using Docker to ensure consistency and portability across different environments.

---

## **Table of Contents**

1. [Technologies Used](#technologies-used)
2. [File Structure](#file-structure)
3. [Setup and Installation](#setup-and-installation)
4. [Usage](#usage)
5. [Environment Variables](#environment-variables)
6. [Contributing](#contributing)
7. [License](#license)

---

## **Technologies Used**

- Docker & Docker Compose
- Node.js (Backend)
- React.js (Frontend)
- MongoDB

---

## **File Structure**

```
project/
â”‚
â”œâ”€â”€ backend/
â”‚   â”œâ”€â”€ Dockerfile
â”‚   â”œâ”€â”€ package.json
â”‚   â””â”€â”€ server.js
â”‚
â”œâ”€â”€ frontend/
â”‚   â”œâ”€â”€ Dockerfile
â”‚   â”œâ”€â”€ package.json
â”‚   â””â”€â”€ src/
â”‚       â””â”€â”€ index.js
â”‚
â”œâ”€â”€ docker-compose.yml
â””â”€â”€ README.md
```

---

## **Setup and Installation**

### Prerequisites
1. Install [Docker](https://www.docker.com/products/docker-desktop).
2. Install [Docker Compose](https://docs.docker.com/compose/install/).

### Steps to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Mayank0851/solution.git
   cd solution
   ```

2. Build and start the services:
   ```bash
   docker-compose up --build
   ```

3. Access the application:
   - **Frontend**: `http://localhost:3000`
   - **Backend**: `http://localhost:5000`
   - **MongoDB**: `mongodb://localhost:27017`

4. To stop the services:
   ```bash
   docker-compose down
   ```

---

## **Environment Variables**

Ensure you create a `.env` file in the backend and frontend directories with the following keys:

### Backend `.env`:
```env
DB=mongodb://<user>:<password>@localhost:27017/<database>
PORT=5000
CLOUD_NAME=<cloudinary_name>
API_KEY=<cloudinary_api_key>
API_SECRET=<cloudinary_api_secret>
```

### Frontend `.env`:
```env
REACT_APP_BASE_URL=http://localhost:5000/api
```

---

## **Contributing**

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Added a new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request��#   n e w r e p o 
 
 
