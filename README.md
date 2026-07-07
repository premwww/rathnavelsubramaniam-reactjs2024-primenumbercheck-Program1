<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Prime Number Checker</title>

</head>

<body>


<div class="container">

    <h2>Prime Number Checker</h2>

    <p>Enter a positive integer to check if it is a prime number.</p>

    

    <!-- User Input -->

    <input type="number" id="numberInput" placeholder="Enter a number" min="1">

    <button onclick="checkPrimeNumber()">Check</button>

    

    <!-- Result Display -->

    <div id="result"></div>

</div>


<script>

function checkPrimeNumber() {

    // 1. Fetch input value and element references

    const inputElement = document.getElementById("numberInput");

    const resultElement = document.getElementById("result");

    const num = parseInt(inputElement.value);


    // 2. Validate user input

    if (isNaN(num)) {

        resultElement.innerText = "Please enter a valid 
