# 🧮 Simple React Calculator (CDN-Based)

## About This Project

This is a minimalist web-based calculator application designed to demonstrate the fundamental concepts of building user interfaces with **React.js** without the need for a complex frontend build tool.

Unlike typical modern React projects that rely on bundlers like Webpack or Vite, this calculator runs entirely from a single HTML file. It leverages **Content Delivery Networks (CDNs)** to load React, ReactDOM, and Babel directly in the browser.

## Why This Approach?

This project serves as an excellent educational example for:
* **Understanding React Fundamentals:** See how React components manage state (`useState`), handle events (`onClick`), and render dynamically.
* **Rapid Prototyping:** Ideal for quickly testing small React ideas or components without any local environment setup.
* **Client-Side Transpilation:** Observe how **Babel** transpiles modern JavaScript (including JSX syntax) and modern JavaScript features in real-time within the browser, making it compatible with older environments.

## Key Technologies Used

* **HTML:** Provides the basic structure of the web page.
* **CSS:** Utilizes basic styling for visual presentation.
* **React:** JavaScript library for building user interfaces.
* **React DOM:** Handles rendering React components to the DOM.
* **Babel (Standalone):** Transpiles JSX and modern JavaScript features directly in the browser.
* **JavaScript:** Powers the calculator's logic and interactivity.
* **Local Storage:** Used for persisting operation history.

## Features

* **Basic Arithmetic Operations:** Supports addition, subtraction, multiplication, and division.
* **Decimal Support:** Handles decimal numbers using a comma (`,`) as the separator.
* **Clear & Clear Entry:** `C` (Clear All) and `CE` (Clear Entry/Delete last input) functionalities.
* **Operation History:** Keeps track of past calculations, persisted using browser's Local Storage.
* **Responsive Design:** Adapts to different screen sizes.

## How to Run This Project

Running this calculator is incredibly simple, as no build process is required:

1.  **Save the file:** Save the `calculadora.html` file to your local computer.
2.  **Open in Browser:** Double-click the `calculadora.html` file, or drag and drop it into any modern web browser (e.g., Chrome, Firefox, Edge).

The calculator will load and run directly in your browser!

## Code Structure Highlights

* **`Calculator` Component:** Manages the calculator's state (`operation`, `result`) and handles all input logic.
* **`CalculatorDisplay` Component:** Renders the current operation and result.
* **`OperationHistory` Component:** Displays a list of previous calculations, leveraging React Context for state management.
* **`CalculatorProvider`:** A React Context Provider that manages the global history state and provides `updateHistory` and `clearHistory` functions to other components.
* **`Text`, `Button`, `Card` Components:** Reusable presentational components for consistent UI elements.

## Potential Enhancements

* **Safer Expression Evaluation:** Replace `eval()` with a dedicated, secure math expression parser library to mitigate potential security risks.
* **Advanced Operations:** Add support for exponents, roots, parentheses, trigonometry, etc.
* **Error Handling:** Improve display of error messages for invalid operations.
* **Keyboard Support:** Add functionality to input numbers and operations using the keyboard.
* **Theming:** Implement different visual themes for the calculator.

This project was developed as part of an activity proposed in the RocketSeat Platform.
