# Frontend Developer Junior Assignment (Mobile-First with GraphQL)

## Objective
Build a **Task Management App** using React, Node.js, TypeScript, GraphQL, and **Material-UI (MUI)**, with a focus on creating a **mobile-first** user experience. The app should allow users to create, update, delete, and view tasks, ensuring the design is optimised for mobile devices first and then scales to larger screens.

## Requirements

### Frontend (React + TypeScript + Material-UI, Mobile-First Design)
- Create a **mobile-first, responsive UI** that allows users to:
  - Add new tasks (with a title, description, and due date).
  - View the list of tasks.
  - Mark tasks as complete/incomplete.
  - Edit or delete tasks.
  - Filter tasks by status (completed, pending).
- Prioritise mobile design first, ensuring that the UI works seamlessly on small screens (mobile phones), then scale up to support tablets and desktops.
- Use **React hooks** and a GraphQL client (e.g., Relay, URQL) to interact with the GraphQL API.
- Apply **TypeScript** for type safety in the React components.
- **Material-UI (MUI):** Use Material-UI components to build the UI. Leverage its pre-designed components and theming capabilities to ensure a consistent and modern look.
- **CSS:** Use media queries to adjust layouts and components for larger screen sizes, following a mobile-first strategy.
  - For example:
    - Mobile: Tasks should be listed vertically, with simple, touch-friendly buttons.
    - Desktop: Tasks could be displayed in a grid or more elaborate layout.
- Keep the design clean and minimal, focusing on usability for touchscreens.

### Backend (Node.js + Express + GraphQL + TypeScript)
- Set up a **GraphQL API** with the following features:
  - Queries:
    - `tasks`: Retrieve the list of all tasks.
    - `task(id: ID!)`: Retrieve a single task by ID.
  - Mutations:
    - `createTask(title: String!, description: String, dueDate: String)`: Create a new task.
    - `updateTask(id: ID!, title: String, description: String, dueDate: String, completed: Boolean)`: Update an existing task.
    - `deleteTask(id: ID!)`: Delete a task by ID.
- Use **TypeScript** on both the server and the GraphQL schema for type safety.
- Use an **in-memory database** (e.g., a simple array of tasks) for this project, or an **in-memory store** with your GraphQL server.

### Mobile-First Considerations
- Ensure all buttons, input fields, and other interactive elements are large enough and spaced appropriately for touch input.
- Consider using features such as **sticky headers**, **bottom navigation**, or **floating action buttons (FABs)** to make the app easy to use on mobile.
- Implement **lazy loading** for tasks to optimise performance on mobile devices.

### Bonus (Optional)
- Add user authentication (e.g., using JWT) to allow users to log in and manage their own tasks.
- Implement **real-time updates** using GraphQL subscriptions, allowing users to see task changes as they happen.
- Deploy the app on a free hosting service (e.g., Heroku for the backend, Vercel/Netlify for the frontend).
- Add **dark mode** support, respecting system preferences (e.g., using `prefers-color-scheme` CSS media queries).

## Deliverables
- A **GitHub repository** with the full code for the project.
- A **README.md** file explaining how to set up and run the application locally.
- A **short demo video** (optional) showing the mobile-first experience and key app features.

## Evaluation Criteria
- Code quality, readability, and structure.
- Proper use of **React**, **GraphQL**, **TypeScript**, and **Material-UI (MUI)**.
- Effective mobile-first design: The app should work flawlessly on mobile and scale well to larger screens.
- User experience: Is the app intuitive and easy to use on mobile devices?
- Bonus: Consideration of real-time capabilities, dark mode, and responsiveness.
