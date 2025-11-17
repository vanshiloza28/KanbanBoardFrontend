🧩 Full Stack Task Collaboration Dashboard - Creative Upaay Web Development Internship Assignment
A full-stack task management dashboard built as part of the Creative Upaay Web Development Internship Assignment. The application is a collaborative platform to manage tasks, events, and subtasks, with real-time updates, due date alerts, and a smooth drag-and-drop interface.

🚀 Project Overview
This dashboard is designed to allow users to:

Add, delete, and update events, tasks, and subtasks
Move tasks across To Do, In Progress, and Done columns via drag and drop
Be notified of tasks that are overdue or nearing due dates
Collaborate in real-time using WebSockets
Maintain state persistently using Redux with LocalStorage
Authenticate securely with JWT
⚡ Implemented all Level 1 features and 5/7 Level 2 optional functionalities as outlined in the assignment.

🛠️ Tech Stack
Frontend
React.js
Tailwind CSS – for responsive and modern UI
Redux – for state management
LocalStorage – for persisting Redux state
Framer Motion – for smooth animations (if used)
Backend
Node.js + Express.js
Prisma ORM – for database interactions
PostgreSQL – relational database
JWT – for user authentication
Socket.IO – for real-time communication
hosted on render
📦 Database Schema
User
Event → userId (FK)
Task → eventId (FK)
Subtask → taskId (FK)
🔑 Core Features
✅ Level 1 - Implemented
 Responsive dashboard layout from Figma
 Add/Delete tasks dynamically
 Move tasks between columns (To Do / In Progress / Done)
 Filter tasks
 Redux state management with LocalStorage
 Drag-and-drop functionality
🌟 Level 2 - Implemented
 JWT Authentication – secure login/signup via HTTP requests
 Due Date & Reminder – notifications for overdue/close-to-due tasks
 Subtasks – nested task management
 Socket.IO Integration – real-time updates on tasks/events/subtasks
 Drag-and-drop (bonus repetition from Level 1)
🧪 Not implemented: Customizable Task Fields, Activity Logs

project deployed - https://kanban-board-frontend-y74a.vercel.app/

⚠️ Deployment Note Due to high latency and cold start times on free hosting platforms (like Vercel and Render), the live demo may experience delays in loading or inconsistent performance. For the best experience, it's recommended to run the project locally by following the instructions in the How to Run Locally section above.

1. Clone the backend Repository - run locally
git clone https://github.com/soham-0-0-7/KanbanBoardBackend.git
cd KanbanBoardBackend
npm install
create a .env file with the variables

DATABASE_URL - url of the online/local postgres data base you want to use.
JWT_SECRET - secret key value
npx prisma migrate dev --name initial_migration
npm run start
2. Clone the frontend Repository - run locally
git clone https://github.com/soham-0-0-7/KanbanBoardFrontend.git
cd KanbanBoardFrontend
npm install
create a .env file with the variables

VITE_API_AUTH_URL - url for where your backend is hosted / listening for login, signup requests.
VITE_SOCKET_URL - url for where your socket interacts.
npm run dev
React + Vite
This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

@vitejs/plugin-react uses Babel for Fast Refresh
@vitejs/plugin-react-swc uses SWC for Fast Refresh
Expanding the ESLint configuration
If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the TS template for information on how to integrate TypeScript and typescript-eslint in your project.
