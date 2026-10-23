# Fancy Store – React Frontend

The React frontend for the **Fancy Store Microservices Project**, a learning project based on Google's Monolith to Microservices codelab.

This application provides the frontend interface and communicates with the Orders and Products services through configured API endpoints.

## Features

* React-based frontend.
* Integration with Orders and Products services.
* Environment-based API configuration.
* Development and production build support.

## Tech Stack

* React.js
* JavaScript
* Node.js and npm
* HTML and CSS

## Project Structure

```text
react-app/
├── public/
├── src/
├── package.json
├── package-lock.json
├── .env.monolith
└── README.md
```

*Note: The exact files and folders may vary depending on the project configuration.*

## Prerequisites

Install the following before running the application:

* Node.js
* npm

## Getting Started

### 1. Navigate to the frontend directory

```bash
cd react-app
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure API endpoints

Configure the appropriate environment settings for your deployment.

For the monolith configuration, the API paths are:

```text
REACT_APP_ORDERS_URL=/service/orders
REACT_APP_PRODUCTS_URL=/service/products
```

Ensure the configuration matches the environment in which the application will run.

### 4. Run the development server

```bash
npm start
```

Open `http://localhost:3000` in your browser.

### 5. Create a production build

```bash
npm run build
```

This generates an optimized production build in the `build/` directory.

## Available Scripts

| Command         | Description                     |
| --------------- | ------------------------------- |
| `npm start`     | Starts the development server.  |
| `npm test`      | Runs the configured test suite. |
| `npm run build` | Creates a production build.     |

## Deployment

The frontend can be built for deployment to a suitable web server or cloud hosting environment.

For microservices deployment, configure the API endpoints and routing to match the Orders and Products services.

## Related Project Components

* `monolith/` – Original monolithic application.
* `microservices/` – Microservices implementation.
* `react-app/` – React frontend.

## Acknowledgment

This project is based on the learning material from Google's Monolith to Microservices codelab.

The repository is intended for learning and portfolio purposes. A running deployment requires the appropriate application configuration and infrastructure.

