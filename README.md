# JavaScript Calculator
This is a simple calculator built with HTML, CSS, and JavaScript for learning purposes. It handles simple arithmetic operations and is ideal for practicing JavaScript skills.

## Table of Contents

- [Features](#features)
- [Deployed Application](#deployed-application)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [License](#license)
- [Contributing](#contributing)
- [Credits](#credits)
- [Contacts](#contacts)

## Features

- Addition, subtraction, multiplication, and division operations.
- Clear button to reset the calculator display.
- Responsive design for use on various devices.

## Deployed Calculator

Check out the live application [here](https://heshbon.github.io/JS-calculator/).

## Technologies Used

- HTML
- CSS
- JavaScript

2. Navigate to the project directory
    cd JS-calculator
3. Open index.html in your browser

## Usage
Use the calculator by clicking the buttons to perform arithmetic operations. The result will be displayed on the screen.

HTML Structure

The HTML file contains the structure of the calculator:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>JS Calculator</title>
  <link rel="stylesheet" href="style.css">
  <script src="index.js" defer></script>
</head>
<body>
  <div id="calculator">
    <input id="display" readonly>
    <div id="keys">
      <button onclick="appendToDisplay('+')" class="operator-btn">+</button>
      <button onclick="appendToDisplay('7')">7</button>
      <button onclick="appendToDisplay('8')">8</button>
      <button onclick="appendToDisplay('9')">9</button>
      <button onclick="appendToDisplay('-')" class="operator-btn">-</button>
      <button onclick="appendToDisplay('4')">4</button>
      <button onclick="appendToDisplay('5')">5</button>
      <button onclick="appendToDisplay('6')">6</button>
      <button onclick="appendToDisplay('*')" class="operator-btn">*</button>
      <button onclick="appendToDisplay('1')">1</button>
      <button onclick="appendToDisplay('2')">2</button>
      <button onclick="appendToDisplay('3')">3</button>
      <button onclick="appendToDisplay('/')" class="operator-btn">/</button>
      <button onclick="appendToDisplay('0')">0</button>
      <button onclick="appendToDisplay('.')">.</button>
      <button onclick="calculate()">=</button>
      <button onclick="clearDisplay()" class="operator-btn">C</button>
    </div>
  </div>
</body>
</html>

CSS Styling

The CSS file contains the styles for the calculator:
body {
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: hsl(0, 0%, 95%);
}

#calculator {
  font-family: Arial, sans-serif;
  background-color: hsl(0, 0%, 15%);
  border-radius: 15px;
  max-width: 500px;
  overflow: hidden;
}

#display {
  width: 100%;
  padding: 20px;
  font-size: 5rem;
  text-align: left;
  border: none;
  background-color: hsl(0, 0%, 25%);
  color: white;
}

#keys {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 10px;
  padding: 25px;
}

button {
  width: 100px;
  height: 100px;
  border-radius: 50px;
  border: none;
  background-color: hsl(200, 20%, 40%);
  color: white;
  font-size: 3rem;
  font-weight: bold;
  cursor: pointer;
}

button:hover {
  background-color: hsl(200, 20%, 50%);
}

button:active {
  background-color: hsl(200, 20%, 60%);
}

.operator-btn {
  background-color: hsl(35, 100%, 55%);
}

.operator-btn:hover {
  background-color: hsl(35, 100%, 65%);
}

.operator-btn:active {
  background-color: hsl(35, 100%, 75%);
}

JavaScript Functionality

The JavaScript file contains the functionality for the calculator:
// Calculator Program

const display = document.getElementById("display");

function appendToDisplay(input) {
  display.value += input;
}

function clearDisplay() {
  display.value = "";
}

function calculate() {
  try {
    display.value = eval(display.value);
  } catch (error) {
    display.value = "Error";
  }
}

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT) - see the [LICENSE](LICENSE) file for details.

## Contributing

    1. Fork the repository
    2. Create your feature branch
    3. Commit your changes
    4. Push to the branch
    5. Open a pull request

## Credits

- Built by Hesbon Kipchirchir <[Heshbon](https://github.com/Heshbon)>

## Contacts
<u>hesskip@gmail.com</u>



