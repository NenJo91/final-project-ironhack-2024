# ToDo Application

This is a Vue.js-based ToDo application that utilizes Pinia for state management and Vue Router for navigation. The application allows users to manage their tasks, including adding new tasks, viewing all tasks, marking tasks as completed, and deleting tasks. Users can also register and log in to the application.

## Table of Contents

- [ToDo Application](#todo-application)
  - [Table of Contents](#table-of-contents)
  - [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
    - [Running the Application](#running-the-application)
  - [Project Structure](#project-structure)
    - [Components](#components)
      - [HelloWorld.vue](#helloworldvue)
      - [PersonalRouter.vue](#personalroutervue)
      - [HomePage.vue](#homepagevue)
      - [AboutPage.vue](#aboutpagevue)
      - [AllTasksPage.vue](#alltaskspagevue)
      - [CompletedTasksPage.vue](#completedtaskspagevue)
      - [AddTaskPage.vue](#addtaskpagevue)
      - [AuthPage.vue](#authpagevue)
      - [SignIn.vue](#signinvue)
      - [SignUp.vue](#signupvue)
    - [Stores](#stores)
      - [taskStore.js](#taskstorejs)
      - [userStore.js](#userstorejs)
    - [Routing](#routing)
  - [Where to Go From Here?](#where-to-go-from-here)
    - [Styling Enhancements](#styling-enhancements)
    - [Task Management Enhancements](#task-management-enhancements)
    - [User Management Enhancements](#user-management-enhancements)
    - [Additional Features](#additional-features)
    - [Third-Party Libraries](#third-party-libraries)
    - [Local Storage Enhancements](#local-storage-enhancements)

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js installed on your machine.
- npm (Node Package Manager) or yarn installed.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/todo-app.git
   cd todo-app
   ```
2. Install the dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

### Running the Application

To start the development server, run:

```bash
npm run dev
# or
yarn dev
```

This will start the application and a route will be provided to you in the integrated terminal.

## Project Structure

### Components

#### HelloWorld.vue

Displays a welcome message.

#### PersonalRouter.vue

Provides navigation links for the application.

#### HomePage.vue

Displays the home view with a counter example using Pinia.

#### AboutPage.vue

Displays information about the application.

#### AllTasksPage.vue

Displays all tasks and allows marking tasks as completed or deleting them.

#### CompletedTasksPage.vue

Displays completed tasks.

#### AddTaskPage.vue

Allows users to add new tasks.

#### AuthPage.vue

Serves as a parent component for authentication-related nested routes.

#### SignIn.vue

Handles the sign-in process.

#### SignUp.vue

Handles the sign-up process.

### Stores

#### taskStore.js

Manages the state of tasks, including adding, marking as completed, and deleting tasks.

#### userStore.js

Manages user authentication and profile information, including registering, signing in, and signing out.

### Routing

The routing configuration is defined in `router.js`. The application uses Vue Router to navigate between different pages and includes nested routes for authentication.

## Where to Go From Here?

Here are 20 possible updates and enhancements that beginners can work on to improve this application::

### Styling Enhancements

1. **Styling Enhancements**: Improve the overall styling using CSS or a framework like Tailwind CSS.
   - **CSS Grid/Flexbox**: Use CSS Grid or Flexbox to create a responsive layout.
   - **Variables**: Use CSS variables for consistent theming and easy updates.
   - **Animations**: Add subtle animations for interactions like button clicks or page transitions.
   - **Hover Effects**: Add hover effects to buttons and links to improve interactivity.
   - **Fonts and Icons**: Integrate Google Fonts for custom typography and use a library like Font Awesome for icons.
2. **Responsive Design**: Make the application responsive so it looks good on mobile devices.
   - **Media Queries**: Use media queries to adjust the layout and styling for different screen sizes.
   - **Mobile Menu**: Implement a hamburger menu for mobile navigation.
   - **Grid Adjustments**: Change the number of columns or layout for smaller screens.
3. **Dark Mode**: Add a toggle for dark mode.
   - **CSS Variables**: Use CSS variables to easily switch between light and dark themes.
   - **Transition Effects**: Add smooth transition effects when toggling between themes.

### Task Management Enhancements

5. **Task Editing**: Add functionality to edit existing tasks.
6. **Task Due Dates**: Allow users to add due dates to tasks.
7. **Task Prioritization**: Implement a priority system for tasks (e.g., high, medium, low).
8. **Search Functionality**: Add a search bar to filter tasks by title or description.
9. **Sort Tasks**: Enable sorting of tasks by due date, priority, or completion status.
10. **Task Categories**: Allow users to categorize tasks (e.g., Work, Personal, Shopping).
11. **Subtasks**: Enable the creation of subtasks within a task.
12. **Recurring Tasks**: Allow users to set tasks to recur daily, weekly, or monthly.
13. **Task Attachments**: Let users attach files or images to tasks.
14. **Task Comments**: Add a commenting system within tasks for additional notes or collaboration.
15. **Drag and Drop**: Implement drag-and-drop functionality for task reordering.

### User Management Enhancements

16. **User Profile Page**: Create a user profile page where users can update their information.

### Additional Features

18. **Notifications**: Implement notifications to remind users of upcoming tasks or deadlines.
19. **Progress Tracking**: Show a progress bar indicating the completion percentage of all tasks.
    s

### Third-Party Libraries

21. **Axios**: Use Axios for handling HTTP requests to a backend server or external APIs.
22. **Lodash**: Integrate Lodash for utility functions to simplify data manipulation.
23. **Moment.js or Date-fns**: Use Moment.js or Date-fns for date and time manipulation.
24. **Vue Draggable**: Implement Vue Draggable for drag-and-drop functionality within lists.
25. **Vuelidate or VeeValidate**: Add form validation using Vuelidate or VeeValidate to enhance user input handling.
26. **Toastification**: Implement Toastification for showing toast notifications to users.
27. **Vuex Persist**: Use Vuex Persist to persist the state of the application across page reloads.
28. **Chart.js or ECharts**: Integrate Chart.js or ECharts for data visualization and analytics.
29. **Vue-i18n**: Add Vue-i18n for internationalization and localization support.

### Local Storage Enhancements

Leveraging localStorage can significantly improve the user experience by persisting data across sessions. Here are some updates and enhancements you can make using localStorage to save key-value pairs, such as tasks and user profiles:

1. **Persist User Sessions**: Save user session data in localStorage to keep users logged in even after refreshing the page.

   - **Example**: When a user logs in, store their session token and user ID in localStorage. On page load, check localStorage for these values and automatically log the user in if they exist.

2. **Store Tasks Locally**: Save tasks to localStorage so that they persist across page reloads.

   - **Example**: Whenever a task is added, edited, or deleted, update the tasks in localStorage. On page load, retrieve the tasks from localStorage and populate the task list.

3. **User Profile Information**: Save user profile details such as email, username, and preferences in localStorage.

   - **Example**: When a user updates their profile information, save the updated details in localStorage. On page load, retrieve and display the profile information.

4. **Theme Preferences**: Store user preferences for light or dark mode in localStorage.

   - **Example**: When a user toggles between light and dark mode, save their preference in localStorage. On page load, apply the saved theme preference.

5. **Task Filters and Sorting**: Persist task filter and sorting options in localStorage.

   - **Example**: Save the user's selected filter (e.g., show only completed tasks) and sorting order (e.g., by due date) in localStorage. On page load, apply these settings automatically.
# final-project-ironhack-2024
