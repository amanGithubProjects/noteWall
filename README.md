# noteWall
# HTML (index.html):

This is the main HTML file that defines the structure of your web page.
It includes a container with a title ("To-Do List") and a form to add new tasks.
The form consists of an input field with the id "task-input" for entering tasks and a button with the id "add-button" to add tasks.
Below the form, there's an unordered list (<ul>) with the id "task-list" where the tasks will be displayed.
It links to an external CSS file (index.css) for styling and an external JavaScript file (index.js) for functionality.

# CSS (index.css):

This file contains the styling rules for the HTML elements.
It sets the font, background color, margins, padding, and styles for various elements to create the visual appearance of the app.
It defines styles for the task list items, including completed tasks and the delete button.

# JavaScript (index.js):

This JavaScript code is wrapped inside a DOM event listener to ensure that the code runs after the HTML has been fully loaded.
It selects the necessary HTML elements using their IDs (task-input, add-button, and task-list) and stores them in variables.
It adds an event listener to the "Add" button (add-button) to trigger the addTask function when clicked.
It adds an event listener to the task list (task-list) to trigger the deleteTask function when a delete button is clicked.

addTask Function:

This function is called when the "Add" button is clicked.
It gets the value entered in the input field (task-input), trims any leading/trailing spaces, and stores it in the taskText variable.
If taskText is not empty, it creates a new list item (<li>) with the task text and a "Delete" button.
The new list item is appended to the task list (task-list), and the input field is cleared.
deleteTask Function:

This function is called when a "Delete" button inside a task list item is clicked.
It checks if the clicked element has the class "delete-button" (indicating it's a delete button).
If it's a delete button, it removes the parent list item (<li>) from the task list, effectively deleting the task.
