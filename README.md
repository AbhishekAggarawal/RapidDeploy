# GitHub Repository Deployment Platform

This project allows users to deploy a GitHub repository directly from a GitHub URL, similar to how Vercel works. The platform utilizes a full stack with technologies like React, Node.js, Express, Redis, AWS S3, and Cloudflare Bucket for seamless and efficient deployment.
# Before proceeding change the rootDir to "./src" and outDir to "./dist" in tsconfig.json
## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- Deploy a GitHub repository directly using the repository URL.
- Monitor and manage deployment processes.
- Store build artifacts using AWS S3 and Cloudflare Bucket.
- Redis is used for caching deployment status and reducing build time.

## Tech Stack

### Frontend:
- **React**: For building the user interface.
  
### Backend:
- **Node.js**: Server-side JavaScript runtime.
- **Express.js**: Web framework for handling HTTP requests.
  
### Caching and Storage:
- **Redis**: Used for managing deployment queues.
- **Cloudflare Bucket**: For storing deployment build files.

## Installation

### Prerequisites
- [Node.js](https://nodejs.org/) (v14.x or higher)
- [Redis](https://redis.io/)
- Cloudflare account for bucket access

### Backend Setup

1. Clone the repository:
    ```bash
    git clone <your-github-repo-url>
    cd your-repo
    ```

2. Install backend dependencies:
    ```bash
    npm install
    ```

3. Set up Redis server and ensure it is running on the default port.


4. Start the backend server:
    ```bash
    tsc -b
    node dist/index.js
    ```

### Frontend Setup

1. Navigate to the frontend directory and install dependencies:
    ```bash
    cd frontend
    npm install
    ```

2. Start the frontend React development server:
    ```bash
    npm run dev
    ```


   <img width="953" alt="Screenshot 2024-10-02 231726" src="https://github.com/user-attachments/assets/e1d4ca6d-7145-4cd6-b6db-d07a20da7321">


