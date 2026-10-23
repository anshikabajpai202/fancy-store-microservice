# Fancy Store — Monolith to Microservices

A cloud-native learning project exploring the transition from a monolithic application to a microservices architecture using Google Cloud technologies.

This project is based on Google's **Monolith to Microservices** codelab and demonstrates how an application can be organized into independent services and deployed using containerization and Kubernetes.

## Project Overview

Traditional monolithic applications combine multiple functionalities into a single application. A microservices architecture separates these functionalities into smaller services that can be developed, deployed, and managed independently.

The Fancy Store project explores this transition through three main components:

* **Monolith:** The original application architecture.
* **Microservices:** Separate Orders and Products services, along with the frontend service.
* **React Frontend:** The user interface that communicates with the application services.

## Architecture

```text
                 ┌──────────────────────┐
                 │     React Frontend   │
                 │      (Frontend)      │
                 └──────────┬───────────┘
                            │
                 ┌──────────┴───────────┐
                 │                      │
       ┌─────────▼────────┐   ┌─────────▼────────┐
       │  Orders Service  │   │ Products Service │
       └──────────────────┘   └──────────────────┘
```

The frontend communicates with the Orders and Products services through configured API endpoints. The exact routing depends on the deployment configuration.

## Technologies Used

* **Frontend:** React.js, JavaScript, HTML, CSS
* **Backend:** Node.js
* **Containers:** Docker
* **Container Orchestration:** Kubernetes
* **Cloud Platform:** Google Cloud Platform (GCP)
* **Container Deployment:** Google Kubernetes Engine (GKE)
* **Build and Image Management:** Google Cloud Build and Container Registry, as used in the original lab workflow
* **Version Control:** Git and GitHub

*The technologies listed describe the project and its original learning workflow. The repository itself does not imply that a cloud deployment is currently running.*

## Repository Structure

```text
fancy-store-microservice/
│
├── monolith/
│   └── Original monolithic application
│
├── microservices/
│   └── Orders, Products, and frontend service code
│
├── react-app/
│   └── React frontend application
│
├── README.md
├── LICENSE
├── CONTRIBUTING.md
└── .gitignore
```

The exact contents of each directory may vary. Refer to the individual folders for their implementation details.

## Getting Started

### Prerequisites

Install the following tools before running the application locally:

* Node.js
* npm
* Git

For cloud deployment, additional requirements include an appropriately configured Google Cloud project, permissions, and the necessary cloud resources.

### Clone the Repository

```bash
git clone https://github.com/anshikabajpai202/fancy-store-microservice.git
```

Navigate to the project directory:

```bash
cd fancy-store-microservice
```

### Run the React Frontend

Navigate to the frontend directory:

```bash
cd react-app
```

Install the dependencies:

```bash
npm install
```

Start the development server:

```bash
npm start
```

Open the local address displayed in the terminal. For a standard Create React App configuration, this is usually:

```text
http://localhost:3000
```

**Note:** Running the frontend alone does not guarantee that Orders and Products functionality will work. The corresponding services and API routing must also be configured and available.

## Cloud Deployment

The original Google Cloud learning workflow explores the following stages:

1. Build a container image for the monolithic application.
2. Create a Kubernetes cluster using Google Kubernetes Engine.
3. Build separate container images for the Orders and Products services.
4. Deploy the services to Kubernetes.
5. Configure the frontend to communicate with the services.
6. Build and deploy the frontend container.

Cloud deployment requires suitable Google Cloud resources, permissions, configuration, and potentially billable services.

The original lab environment may be temporary. Cloning this repository does not recreate the cloud infrastructure or guarantee a live website.

## Learning Outcomes

This project provides practical exposure to:

* Understanding monolithic and microservices architectures.
* Organizing application components into separate services.
* Working with Docker containers and container images.
* Learning Kubernetes deployment concepts.
* Exploring Google Cloud Build and Google Kubernetes Engine.
* Configuring frontend communication with backend services.
* Managing project code using Git and GitHub.

## Acknowledgment

This project is based on Google's **Monolith to Microservices** codelab and is intended for educational and portfolio purposes.

Original learning resource: [Google Codelabs — Monolith to Microservices](https://github.com/googlecodelabs/monolith-to-microservices)

## Author

**Anshika Bajpai**

GitHub: [@anshikabajpai202](https://github.com/anshikabajpai202)

---


