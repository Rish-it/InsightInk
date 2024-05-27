

# InsightInk

This project is a blogging platform named InsightInk, built using the Hono library, Cloudflare, TypeScript, Prisma for the backend, and Tailwind CSS and Vite for the frontend.

## Table of Contents

- [Project Description](#project-description)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Setup](#setup)
- [Configuration](#configuration)
- [Running the Project](#running-the-project)
- [Contributing](#contributing)
- [License](#license)

## Project Description

InsightInk is a feature-rich blogging platform inspired by Medium. Users can create, edit, and delete articles, follow other users, and interact with posts through comments and likes.

## Tech Stack

- **Backend**: Hono, Cloudflare, TypeScript, Prisma
- **Frontend**: Tailwind CSS, Vite

## Features

- User authentication and authorization
- CRUD operations for articles
- Commenting system
- User profiles with follow functionality
- Responsive design

## Setup

### Prerequisites

- Node.js (>= 14.x)
- npm or yarn
- PostgreSQL (for Prisma)

### Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/InsightInk.git
   cd InsightInk
   ```

2. **Install dependencies**:
   ```sh
   # Backend dependencies
   cd backend
   npm install

   # Frontend dependencies
   cd ../frontend
   npm install
   ```

### Configuration

#### Backend

1. **Environment Variables**:
   Create a `.env` file in the `backend` directory and add your configuration:

   ```env
   DATABASE_URL="postgresql://user:password@localhost:5432/mydb"
   JWT_SECRET="your_jwt_secret"
   CLOUD_FLARE_API_KEY="your_cloudflare_api_key"
   ```

2. **Prisma Setup**:
   Initialize Prisma and migrate your database:

   ```sh
   cd backend
   npx prisma init
   npx prisma migrate dev --name init
   ```

#### Frontend

1. **Environment Variables**:
   Create a `.env` file in the `frontend` directory and add your configuration:

   ```env
   VITE_API_URL="http://localhost:3000"
   ```

## Running the Project

1. **Start the Backend**:
   ```sh
   cd backend
   npm run dev
   ```

2. **Start the Frontend**:
   ```sh
   cd frontend
   npm run dev
   ```

3. Open your browser and navigate to `http://localhost:3000` for the frontend and `http://localhost:3001` for the backend (or as configured).

## Contributing

We welcome contributions! Please see our [contributing guidelines](CONTRIBUTING.md) for more information.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to customize this `README.md` file according to your project's specific details and requirements. Make sure to replace placeholder values (like `yourusername`, `your_jwt_secret`, `your_cloudflare_api_key`, etc.) with actual values relevant to your project.
