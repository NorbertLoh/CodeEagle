## Code Eagle

Members:
- Lim Kok Liang
- Billy Ho Cheng En
- Loh Ze Qing Norbert
- Sherwyn Ng Cheng Xin
- Foo Tzie Huang

## Table of Contents
- [Table of Contents](#table-of-contents)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started (dev)](#getting-started-dev)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Credits](#credits)

## Features
- 👤 User Authentication & Authorization
- 💻 Real-time Collaborative Coding Environment
- ▶️ Code Compilation & Execution
- 🕒 Collaboration Session History 
- 📚 Question Database Management

## Tech Stack
- **Frontend:** React, Vite, Mantine UI
- **Auth Router/User Service:** Node.js, Express
- **Questions/Collab/Matching/Code Exec Services:** Python, FastAPI

## Getting Started (dev)
1. Clone the repository into your local machine:
   ```bash
   git clone https://github.com/NorbertLoh/CodeEagle.git
2. Fill in the env variables as per the `.env.dev.example` file in root directory, save as `.env`
3. Run with command from directory root:
   ```bash
   docker-compose --profile dev up --build
   ```

## Usage
1. Go to `http://localhost:5173` to access the Code Eagle frontend.
2. Register a new account or login with Google Sign-In.
3. Explore features like starting collaboration sessions, practicing coding questions, and viewing session history.

## Folder Structure
```python
CodeEagle/
├── frontend/                  # Frontend React application
│   └── peerprep/              # Main Code Eagle application
│       └──...                 # React components, pages, assets, etc.
│
├── services/
│   ├── auth-router/           # User authentication and routing service
│   │   └──...                 # Express server code, routes, controllers, etc.
│   │
│   ├── collaboration-service/ # Real-time collaboration service
│   │   └──...                 # FastAPI server code, WebSocket handlers, etc.
│   │
│   ├── code-exec-service/     # Code compilation and execution service
│   │   └──...                 # FastAPI server code, code execution logic, etc.
│   │
│   ├── matching-service/      # User matching service
│   │   └──...                 # FastAPI server code, matching algorithms, etc.
│   │
│   ├── question-service/      # Question database management service
│   │   └──...                 # FastAPI server code, database models, etc.
│   │
│   ├── user-service/          # User data management service
│   │   └──...                 # Express server code, User data models, etc.
│   │
│   └── y-redis/               # Yjs WebSocket server with Redis persistence
│       └──...                 # Yjs server code, Redis integration, etc.
│
├── .env.example               # Example environment variables file
├── docker-compose.yml         # Docker Compose configuration
└── README.md                  # Project documentation
```

## Credits
This project is developed by Group G37 for the CS3219 course at NUS. Thanks to all members for their contributions to this successful project, as well as the teaching team for their support :)

y-redis service is adapted from: [https://github.com/yjs/y-redis](https://github.com/yjs/y-redis)

## AI Use Summary
Tools Used: Github Copilot (GPT4.1)
- Auto-complete
- Debugging

AI was used for debugging and implementation of scripts: deploy-services.yml, deploy-all-services.sh, deploy-all-services.ps1 
