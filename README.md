# AgileBudhi

AgileBudhi is a cutting-edge web application that combines the power of React, FastAPI, and OpenAI's language models to provide AI-driven project management and digital transformation solutions.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Project Structure](#project-structure)
- [UI Components](#ui-components)
- [Backend API](#backend-api)
- [OpenAI Integration](#openai-integration)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Overview

AgileBudhi is designed to empower organizations in their digital transformation journey by leveraging AI-driven solutions and agile methodologies. Our platform offers a seamless blend of project management tools, AI insights, and cloud services to optimize workflows and drive innovation.

## Features

- AI-Powered Project Management
- Agile Transformation Tools
- Digital Innovation Solutions
- Cloud Services Integration
- Interactive and Responsive UI
- Dark/Light Mode Toggle
- RESTful API with FastAPI
- OpenAI Language Model Integration

## Tech Stack

### Frontend
- React.js
- Material-UI (MUI)
- React Router
- Tailwind CSS

### Backend
- FastAPI
- Python 3.8+
- OpenAI API

### AI/ML
- OpenAI's GPT models

## Getting Started

### Prerequisites

- Node.js (v14+)
- Python (v3.8+)
- pip
- npm or yarn

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/your-username/agilebudhi.git
   cd agilebudhi
   ```

2. Set up the frontend:
   ```
   cd frontend
   npm install
   ```

3. Set up the backend:
   ```
   cd ../backend
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   Create a `.env` file in the `backend` directory and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

5. Start the development servers:
   
   Frontend:
   ```
   cd frontend
   npm start
   ```
   
   Backend:
   ```
   cd backend
   uvicorn app.main:app --reload
   ```

## Project Structure

```
AgileBudhi/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── styles/
│   │   ├── utils/
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── README.md
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── models.py
│   │   ├── schemas.py
│   │   └── ai_utils.py
│   ├── requirements.txt
│   └── .env
├── Market Research/
│   └── Project-Management-Software.md
├── Install.md
└── setup_agilebudhi.sh
```

## UI Components

Our UI is built with React and Material-UI, featuring a modern and intuitive design. Key components include:

- Responsive AppBar with dark/light mode toggle
- Sidebar navigation with custom styled components
- Gradient typography for headings
- Hover-effect cards for services showcase
- Custom styled buttons with gradient backgrounds

For more details, refer to the `HomePage` component in the provided code snippet.

## Backend API

The backend is powered by FastAPI, providing a robust and efficient RESTful API. Key endpoints include:

- `/api/projects`: CRUD operations for projects
- `/api/tasks`: Manage tasks within projects
- `/api/ai/insights`: Generate AI-powered insights for projects
- `/api/analytics`: Retrieve project analytics and metrics

Detailed API documentation is available at `http://localhost:8000/docs` when running the backend server.

## OpenAI Integration

We utilize OpenAI's GPT models to provide AI-driven insights and assistance throughout the project management process. The integration is handled in the `ai_utils.py` file, which includes functions for:

- Generating project summaries
- Providing task recommendations
- Analyzing project risks
- Offering optimization suggestions

## Deployment

For production deployment, we recommend:

1. Building the React frontend:
   ```
   cd frontend
   npm run build
   ```

2. Serving the frontend build with a web server like Nginx

3. Deploying the FastAPI backend with a production ASGI server like Gunicorn

4. Using a reverse proxy to route requests to the frontend and backend


## Contributing

We welcome contributions to AgileBudhi! Please read our contributing guidelines before submitting pull requests.

## License

This project is licensed under the MIT License. See the LICENSE file for details.