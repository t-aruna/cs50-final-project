# cs50-final-project
CS50 Introduction to Computer Science Assignments final project
# Goal Getter

## Project Video
[Watch the Project Video Here](https://youtu.be/iIBIip8Dwxg)

## Description
Goal Getter is a simple yet effective productivity application designed to help users manage their tasks and notes. The application provides a clean and user-friendly interface that allows users to log in, create to-do lists, and jot down notes. By incorporating features like task completion tracking and streak counting, Goal Getter encourages users to stay organized and productive.

## File Structure
The project consists of a single HTML file:

- **`index.html`**: This file serves as the main entry point for the Goal Getter application. It contains all the necessary code to render the user interface and manage user interactions.

### Breakdown of `index.html`

The `index.html` file is structured into several key sections:

1. **HTML Head Section**:
   - The `<head>` section contains metadata about the document, including the character set, viewport settings for responsive design, and the title of the application.
   - A `<style>` block is included for internal CSS styling, which defines the layout, colors, and appearance of various elements within the application.

2. **Body Section**:
   - The body of the document is divided into three main containers:
     - **Login Container**: This section allows users to enter their username and password to log in. It includes:
       - A heading (`<h1>`) prompting users to log in.
       - A form (`<form>`) with input fields for the username and password, and a submit button.
       - A paragraph (`<p>`) to display login messages.
     
     - **To-Do List Container**: Once logged in, users can access this section to manage their tasks:
       - A heading for the to-do list.
       - An input field for adding new tasks and buttons for adding tasks and clearing completed ones.
       - An unordered list (`<ul>`) to display the list of tasks.
       - A streak counter to track the number of consecutive tasks completed.
       - A logout button to exit the application.
     
     - **Notes Container**: This section allows users to write and manage notes:
       - A heading for notes.
       - An input field for adding new notes and a button to submit them.
       - An unordered list (`<ul>`) to display the notes.

3. **JavaScript Section**:
   - A `<script>` block at the end of the body contains all the JavaScript functionality for the application. Key features include:
     - **Login Logic**: Handles user login by validating the input and transitioning to the to-do and notes sections.
     - **Task Management**: Functions to add tasks to the DOM, mark them as completed, and clear completed tasks. Tasks are stored in the browser's local storage to persist between sessions.
     - **Streak Tracking**: Increments or decrements a streak counter based on task completion, providing positive reinforcement to users.
     - **Logout Functionality**: Resets the application state when a user logs out, including clearing the streak counter.
     - **Notes Functionality**: Allows users to add notes that are displayed in a list format.

### Design Choices
Several design choices were made to enhance user experience and functionality:

- **Single Page Application (SPA) Approach**: The use of a single HTML file simplifies the application structure, making it easy to manage and deploy. This design choice is particularly effective for smaller applications where complex routing is unnecessary.
  
- **Internal CSS Styling**: By including CSS directly in the HTML file, the application maintains a lightweight structure. The styles are designed to create a clean, modern look, with a color palette that is easy on the eyes.

- **JavaScript for Interactivity**: The use of JavaScript allows for dynamic interactions without requiring page reloads. This enhances the user experience by providing immediate feedback, such as updating the task list and streak counter in real-time.

- **Local Storage for Data Persistence**: Storing tasks in local storage ensures that users' data is retained even when the browser is closed or refreshed. This feature is crucial for a productivity application, as it allows users to pick up where they left off.

### Future Enhancements
While the current implementation of Goal Getter is functional, there are several enhancements that could be implemented in future iterations:
- **User  Authentication**: Implementing a backend service for user authentication would allow multiple users to have their own accounts and data.
- **Mobile Responsiveness**: Further refining the CSS to ensure the application is fully responsive on mobile devices.
- **Additional Features**: Adding features such as due dates for tasks, priority levels, and reminders could enhance the application's functionality.
- **Analytics Dashboard**: Providing users with insights into their productivity patterns, such as task
