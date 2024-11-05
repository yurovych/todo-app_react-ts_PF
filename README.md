### Todo Application Description

## Brief Description
The Todo Application is a modern task management tool built using React. It allows users to create, manage, and organize their daily tasks efficiently. Leveraging the capabilities of React, the app provides a responsive and intuitive interface for managing todos.

#### Technologies Used

- **HTML** used for structuring the content of the application, including product listings, user authentication forms, and the checkout interface.
- **CSS (SCSS)** employed for styling and layout design, providing a modern look and feel to the application. SCSS allows for nested styles and variables, making the CSS more maintainable.
- **JavaScript(TypeScript)** utilized for adding dynamic behavior to the application, enhancing interactivity. TypeScript provides type safety, making the code more robust and easier to maintain.
- **React** A JavaScript library used for building user interfaces, allowing for the creation of reusable components and efficient rendering of dynamic data.

#### Key Features

1. **User Interaction**: 
   - Users can add new tasks by entering text into an input field. The app validates input to ensure no empty titles are submitted.
   - Each todo item can be marked as completed or active by clicking a checkbox.
   - Users can delete individual tasks or clear all completed tasks with a single click.

2. **Real-Time Updates**: 
   - The application utilizes React's context API to manage state globally. It ensures that any changes in the todo list are reflected immediately across the application.
   - When a user updates a task or its status, the changes are sent to a backend API, ensuring persistent storage of todos.

3. **Error Handling**: 
   - The app provides user feedback through error notifications. If an operation fails (like adding or updating a todo), a relevant error message is displayed for a brief period.
   - There are safeguards to prevent the addition of empty todos and to confirm changes before submitting.

4. **Dynamic Filtering**: 
   - Users can filter the displayed todo list by status: All, Active, or Completed. This feature helps users focus on specific tasks and manage their workflow effectively.

#### Application Structure

- **HTML Structure**: The application starts with a simple HTML layout, setting the stage for rendering the React components. The main rendering occurs within a `<div>` with the ID `root`.
  
- **React Components**:
  - **App**: The main component that holds the application logic and state. It retrieves todos from the server and handles user interactions.
  - **TodosProvider**: A context provider that encapsulates state management for todos, error messages, and submission status.
  - **TodosList**: Displays the list of todos. It uses the `TodosItem` component to render individual items.
  - **TodosItem**: Represents a single todo, including edit functionality and a delete button.
  - **TodosFilter**: Provides options to filter the todos displayed based on their completion status.
  - **ErrorNotification**: Shows error messages when operations fail, improving user experience by providing feedback.

- **Styling**: The app employs Bulma CSS framework and Font Awesome icons for styling and user interface enhancements, ensuring a clean and modern appearance.

- **API Integration**: The application interacts with a RESTful API to fetch, add, update, and delete todos. This functionality is abstracted in the `api/todos.js` file, allowing for easy modifications and expansions.

#### Conclusion

This Todo Application is a feature-rich, user-friendly tool designed for managing tasks effectively. It highlights the power of React for building interactive UIs while maintaining a clean separation of concerns through components and context. Whether used for personal task management or team projects, this application provides a robust solution for staying organized and productive.

## Links
- **Preview**: [Project Live Preview](https://yurovych.github.io/todo-app_react-ts_PF/)

#### Additional Instructions

To run the project locally:

1. Use Node v20 or higher.
2. Copy the repository url.
3. Clone the repository to your directory ('git clone <url>').
4. Ensure that you have a live server extension or tool to preview the HTML file.
5. Run 'npm install'.
6. Open `index.html` in the browser by running 'npm start' in terminal.