
# Express-React-TS-Template

A monorepo template for a full-stack application combining **Express** (backend) and **React** (frontend) with **TypeScript** and **Tailwind CSS**. This setup provides an efficient environment for building and testing both the server and client sides together.

## Project Structure

- **root**: Contains the main configuration and scripts for running both the server and client concurrently.
- **client**: React application with TypeScript and Tailwind CSS for building the frontend.
- **server**: Express server with TypeScript for handling the backend API.

## Requirements

- **Node.js** (>= 14.x recommended)
- **npm**

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/saharulit/express-react-ts-template.git
cd express-react-ts-template
```

### 2. Install Dependencies

Using npm workspaces, you can install all dependencies in the root directory:

```bash
npm install
```

### 3. Run the Project

The following command will run both the **server** and **client** concurrently:

```bash
npm start
```

- **Client**: Runs on `http://localhost:5173`
- **Server**: Runs on `http://localhost:3000`

### 4. Build the Project

To build both the **client** and **server**:

```bash
npm run build -w client
npm run build -w server
```

### 5. Testing

To run tests for both the client and server:

```bash
npm test
```

## Scripts

Here are the main scripts available:

- **Root**:
  - `npm start`: Runs both the client and server in development mode.
  - `npm test`: Runs tests for both client and server concurrently.

- **Client**:
  - `npm run dev -w client`: Starts the client in development mode.
  - `npm run build -w client`: Builds the client for production.
  - `npm run lint -w client`: Lints the client code.
  - `npm run preview -w client`: Previews the built client application.
  - `npm test -w client`: Runs the client tests with Vitest.

- **Server**:
  - `npm run dev -w server`: Starts the server in development mode with `ts-node`.
  - `npm run start -w server`: Runs the compiled server code.
  - `npm test -w server`: Runs server tests with Jest.
