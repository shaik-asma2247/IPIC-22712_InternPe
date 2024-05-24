Intern ID : # IPIC-22712
Intern Name : SHAIK ASMA

Company Name : InternPe
Task : Simple Calculator

The task involves creating a simple web-based calculator using HTML, CSS, and JavaScript. The code provided consists of three main parts: the HTML structure, the CSS styling, and the JavaScript functionality.
Here is a detailed description of each part:

--->  HTML

The HTML code defines the layout of the calculator. It includes a container for the calculator, a display area for showing the input and output, and a set of keys for the user to interact with.

- **`<div class="app">`**: The main container for the application.
- **`<div class="calculator">`**: The container for the calculator itself.
  - **`<div class="display">`**: The display area showing the current input and the result.
    - **`<div class="content">`**: Contains the input and output elements.
      - **`<div class="input">`**: Displays the current input.
      - **`<div class="output">`**: Displays the result of the calculation.
  - **`<div class="keys">`**: The container for all the calculator keys.
    - **Keys (`<div class="key">`)**: Individual buttons for digits, operators, and actions. Each key has a `data-key` attribute specifying its function.

----> CSS
The CSS code provides the styling for the calculator, ensuring it has a modern look and is responsive.

- **Global Styles**: Basic styles for margin, padding, box-sizing, and font.
- **`body`**: Sets the background image and its properties.
- **`.app`**: Centers the calculator on the screen.
- **`.calculator`**: Styles the main calculator container, including background color, size, and layout.
- **`.display`**: Styles the display area, including padding, text alignment, and color.
  - **`.input`**: Styles the input text.
  - **`.output`**: Styles the output/result text.
- **`.keys`**: Styles the keys container, including grid layout and padding.
  - **`.key`**: Styles individual keys, including size, background color, and hover effects.
  - **`.key.operator`**: Specific styles for operator keys.
  - **`.key.action`**: Specific styles for action keys (clear, backspace, etc.).

----> JavaScript

The JavaScript code handles the functionality of the calculator, including user interactions and calculations.

- **`const keys = document.querySelectorAll('.key');`**: Selects all the keys.
- **Event Listener for Each Key**: Adds a click event listener to each key to handle different types of input (clear, backspace, equals, brackets, operators, and digits).
  - **`if (value == "clear")`**: Clears the input and output.
  - **`else if (value == "backspace")`**: Deletes the last character of the input.
  - **`else if (value == "=")`**: Evaluates the input and displays the result.
  - **`else if (value == "brackets")`**: Adds opening or closing brackets appropriately.
  - **`else`**: Adds digits or operators to the input if valid.
- **Helper Functions**:
  - **`CleanInput(input)`**: Formats the input for display, adding appropriate styles to operators and brackets.
  - **`CleanOutput(output)`**: Formats the output, adding commas for thousands separators and handling decimals.
  - **`ValidateInput(value)`**: Validates the input to prevent invalid sequences (e.g., two consecutive operators).
  - **`PerpareInput(input)`**: Prepares the input for evaluation, handling percentage calculations.

--->  Conclusion

The provided code sets up a fully functional calculator with a visually appealing interface. The HTML lays out the structure, the CSS styles it, and the JavaScript adds interactivity and logic for performing calculations. The calculator handles basic arithmetic operations, including addition, subtraction, multiplication, division, and percentages, and allows for clearing input and deleting the last character.
