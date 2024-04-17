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
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Colorful Calculator</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: white;
    }
    .calculator {
        width: 300px;
        margin: 50px auto;
        border: 1px solid #ccc;
        border-radius: 5px;
        background-color: whitesmoke;
        padding: 20px;
    }
    h1 {
        text-align: center;
        color: #333;
    }
    input[type="button"] {
        width: 50px;
        height: 50px;
        margin: 5px;
        font-size: 18px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
    }
    input[type="text"] {
        width: 100%;
        height: 50px;
        margin-bottom: 10px;
        font-size: 24px;
        text-align: right;
        border: none;
        border-radius: 5px;
        padding: 5px;
    }
</style>
</head>
<body>

<div class="calculator">
    <h1 >Yadhav G.P</h1>
    <h1 >212223230247</h1>
    <input type="text" id="display" class="result" readonly>
    <br>
    <input type="button" value="7" onclick="appendToDisplay('7')" style="background-color: #ffcc00;">
    <input type="button" value="8" onclick="appendToDisplay('8')" style="background-color: #33ccff;">
    <input type="button" value="9" onclick="appendToDisplay('9')" style="background-color: #ff6666;">
    <input type="button" value="/" onclick="appendToDisplay('/')" style="background-color: #99cc33;">
    <br>
    <input type="button" value="4" onclick="appendToDisplay('4')" style="background-color: #ff9933;">
    <input type="button" value="5" onclick="appendToDisplay('5')" style="background-color: #ff6666;">
    <input type="button" value="6" onclick="appendToDisplay('6')" style="background-color: #33ccff;">
    <input type="button" value="*" onclick="appendToDisplay('*')" style="background-color: #ffcc00;">
    <br>
    <input type="button" value="1" onclick="appendToDisplay('1')" style="background-color: #33ccff;">
    <input type="button" value="2" onclick="appendToDisplay('2')" style="background-color: #ffcc00;">
    <input type="button" value="3" onclick="appendToDisplay('3')" style="background-color: #ff9933;">
    <input type="button" value="-" onclick="appendToDisplay('-')" style="background-color: #99cc33;">
    <br>
    <input type="button" value="0" onclick="appendToDisplay('0')" style="background-color: #ff6666;">
    <input type="button" value="." onclick="appendToDisplay('.')" style="background-color: #ffcc00;">
    <input type="button" value="=" onclick="calculate()" style="background-color: #99cc33;">
    <input type="button" value="+" onclick="appendToDisplay('+')" style="background-color: #ff9933;">
    <br>
    <input type="button" value="C" onclick="clearDisplay()" style="background-color: #ff6666;">
</div>
<script>
    function appendToDisplay(value) {
        document.getElementById('display').value += value;
    }

    function clearDisplay() {
        document.getElementById('display').value = '';
    }

    function calculate() {
        var expression = document.getElementById('display').value;
        var result = eval(expression);
        document.getElementById('display').value = result;
    }
</script>

</body>
</html>

## OUTPUT:
![Screenshot 2024-04-17 141113](https://github.com/iamyadhav/Calc/assets/147139713/2fead762-8e48-4eab-9c58-d9950a9cbcbd)
![Screenshot 2024-04-17 141132](https://github.com/iamyadhav/Calc/assets/147139713/b673d31d-fdf8-44f4-8799-22d2abb35940)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
