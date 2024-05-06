# Ex.08 Design of a Standard Calculator
## Date:

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Calculator</title>
    <link rel="stylesheet" href="stylee.css">
</head>
<body>
    <h2 class="text">VISHINU H(212223220124)</h2><br>
    <div class="calculator">
        <h1>Calculator</h1>
        <input type="text" id="display" disabled>
        <div class="buttons">
            <button onclick="appendToDisplay('1')">1</button>
            <button onclick="appendToDisplay('2')">2</button>
            <button onclick="appendToDisplay('3')">3</button>
            <button onclick="appendToDisplay('+')">+</button>
            <button onclick="appendToDisplay('4')">4</button>
            <button onclick="appendToDisplay('5')">5</button>
            <button onclick="appendToDisplay('6')">6</button>
            <button onclick="appendToDisplay('-')">-</button>
            <button onclick="appendToDisplay('7')">7</button>
            <button onclick="appendToDisplay('8')">8</button>
            <button onclick="appendToDisplay('9')">9</button>
            <button onclick="appendToDisplay('*')">*</button>
            <button onclick="appendToDisplay('0')">0</button>
            <button onclick="appendToDisplay('%')">%</button>
            <button onclick="appendToDisplay('^')">^</button>
            <button onclick="appendToDisplay('(')">(</button>
            <button onclick="appendToDisplay(')')">)</button>
            <button onclick="calculate()">=</button>
            <button onclick="appendToDisplay('/')">/</button>
            <button onclick="clearDisplay()">C</button>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>

```
CSS
```
body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column; /* Added to align items vertically */
    height: 100vh;
    background-color: #93baec;
}

h2.text {
    font-size: 20px; /* Adjust font size as needed */
    color: #1b191c;
    margin-bottom: 20px; /* Add some space below the h2 tag */
}

.calculator {
    background-color: #e2f048;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(21, 14, 14, 0.1);
}

#display {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    font-size: 24px;
    text-align: right;
    color: #0f0f0e;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

button {
    padding: 15px;
    font-size: 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #080606;
}

```
JS
```
let display = document.getElementById('display');

function appendToDisplay(value) {
    display.value += value;
}

function clearDisplay() {
    display.value = '';
}

function calculate() {
    try {
        display.value = eval(display.value);
    } catch (error) {
        display.value = 'Error';
    }
}

```

## OUTPUT:
![Screenshot 2024-05-06 085124](https://github.com/VisHinu24/Calc/assets/144244396/712450b8-0119-46af-a07e-aa118ffdce22)
![Screenshot 2024-05-06 085142](https://github.com/VisHinu24/Calc/assets/144244396/068d551e-cfac-4aa7-9247-1501595daf7c)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
