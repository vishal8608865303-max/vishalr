<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Assignment 3</title>

<style>
    *{
        margin:0;
        padding:0;
        box-sizing:border-box;
        font-family: Arial, sans-serif;
    }

    body{
        background:#f4f4f4;
        padding:20px;
    }

    .container{
        max-width:900px;
        margin:auto;
        background:white;
        padding:20px;
        border-radius:10px;
        box-shadow:0 0 10px rgba(0,0,0,0.2);
    }

    header{
        text-align:center;
        background:#0077cc;
        color:white;
        padding:20px;
        border-radius:10px;
    }

    header h1{
        margin-bottom:10px;
    }

    section{
        margin-top:30px;
        padding:20px;
        background:#f9f9f9;
        border-radius:10px;
    }

    h2{
        margin-bottom:15px;
        color:#0077cc;
    }

    label{
        font-weight:bold;
        display:block;
        margin-top:10px;
    }

    input{
        width:100%;
        padding:10px;
        margin-top:5px;
        border:1px solid #ccc;
        border-radius:5px;
    }

    button{
        margin-top:15px;
        padding:10px 20px;
        background:#0077cc;
        color:white;
        border:none;
        border-radius:5px;
        cursor:pointer;
    }

    button:hover{
        background:#005fa3;
    }

    .result{
        margin-top:15px;
        font-size:18px;
        font-weight:bold;
    }

    .weak{
        color:red;
    }

    .medium{
        color:orange;
    }

    .strong{
        color:green;
    }

    footer{
        margin-top:30px;
        text-align:center;
        padding:15px;
        background:#0077cc;
        color:white;
        border-radius:10px;
    }
</style>
</head>

<body>

<div class="container">

<header>
    <h1>JavaScript Mini Applications</h1>

    <p><strong>Student Name:</strong> Vishal M</p>
    <p><strong>Roll Number:</strong> S24422</p>
    <p><strong>Department:</strong> Bachelor Of Computer Application (BCA)</p>
    <p><strong>Batch:</strong> 2024 - 2027</p>
    <p><strong>College Name:</strong> Cardamom Planters' Association College</p>
</header>

<!-- AGE CALCULATOR -->

<section>
    <h2>1. Age Calculator</h2>

    <label>Enter Your Date of Birth:</label>
    <input type="date" id="dob">

    <button onclick="calculateAge()">Calculate Age</button>

    <div class="result" id="ageResult"></div>
</section>

<!-- PASSWORD CHECKER -->

<section>
    <h2>2. Password Strength Checker</h2>

    <label>Enter Password:</label>
    <input type="password" id="password" onkeyup="checkPassword()">

    <button onclick="togglePassword()">Show / Hide Password</button>

    <div class="result" id="passwordResult"></div>
</section>

<footer>
    Foundations of Full Stack Web Development using Python & Django
</footer>

</div>

<script>

function calculateAge(){

    let dob = document.getElementById("dob").value;
    let result = document.getElementById("ageResult");

    if(dob == ""){
        result.innerHTML = "Please enter your date of birth.";
        result.style.color = "red";
        return;
    }

    let birthDate = new Date(dob);
    let today = new Date();

    let years = today.getFullYear() - birthDate.getFullYear();
    let months = today.getMonth() - birthDate.getMonth();
    let days = today.getDate() - birthDate.getDate();

    if(days < 0){
        months--;
        days += 30;
    }

    if(months < 0){
        years--;
        months += 12;
    }

    result.style.color = "green";
    result.innerHTML =
    "Age: " + years + " Years, " +
    months + " Months, " +
    days + " Days";
}

function checkPassword(){

    let password = document.getElementById("password").value;
    let result = document.getElementById("passwordResult");

    let strength = 0;

    if(password.length >= 8){
        strength++;
    }

    if(/[A-Z]/.test(password)){
        strength++;
    }

    if(/[a-z]/.test(password)){
        strength++;
    }

    if(/[0-9]/.test(password)){
        strength++;
    }

    if(/[^A-Za-z0-9]/.test(password)){
        strength++;
    }

    if(password.length == 0){
        result.innerHTML = "";
    }
    else if(strength <= 2){
        result.innerHTML = "Weak Password";
        result.className = "result weak";
    }
    else if(strength <= 4){
        result.innerHTML = "Medium Password";
        result.className = "result medium";
    }
    else{
        result.innerHTML = "Strong Password";
        result.className = "result strong";
    }
}

function togglePassword(){

    let passwordField = document.getElementById("password");

    if(passwordField.type === "password"){
        passwordField.type = "text";
    }
    else{
        passwordField.type = "password";
    }
}

</script>

</body>
</html>