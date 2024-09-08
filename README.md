# kel<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. Kelum Amarasighe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f8ff;
            color: #333;
        }
        header {
            background-color: #4a90e2;
            color: white;
            text-align: center;
            padding: 1em 0;
        }
        .container {
            padding: 20px;
        }
        h1 {
            margin: 0;
        }
        .contact-info {
            background-color: #eaf2f8;
            padding: 15px;
            border-radius: 5px;
            margin: 15px 0;
        }
        .contact-info p {
            margin: 5px 0;
        }
        .form-section {
            margin-top: 20px;
        }
        .form-section h2 {
            margin-top: 0;
        }
        form {
            background-color: #eaf2f8;
            padding: 15px;
            border-radius: 5px;
            margin-top: 10px;
        }
        label {
            display: block;
            margin-top: 10px;
        }
        input, select {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        button {
            background-color: #4a90e2;
            color: white;
            border: none;
            padding: 10px;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background-color: #357abd;
        }
    </style>
</head>
<body>

<header>
    <h1>Dr. Kelum Amarasighe</h1>
    <p>General Practitioner of Family Medicine</p>
</header>

<div class="container">
    <div class="contact-info">
        <p><strong>Clinic Address:</strong> Halpe Junction, Kotadeniyawa Road, Mirigama</p>
        <p><strong>Clinic Hours:</strong> Opens from 6:30 PM onwards, all days except Sundays and Poya Days</p>
        <p><strong>Contact Number:</strong> 0710362650</p>
        <p><strong>Email:</strong> <a href="mailto:drkelamara@gmail.com">drkelamara@gmail.com</a></p>
    </div>

    <div class="form-section">
        <h2>Patient Details</h2>
        <form>
            <label for="regNumber">Registration Number:</label>
            <input type="text" id="regNumber" name="regNumber">
            
            <label for="nicNumber">National ID Number:</label>
            <input type="text" id="nicNumber" name="nicNumber">
            
            <label for="date">Date:</label>
            <input type="date" id="date" name="date">
            
            <label for="age">Age:</label>
            <input type="number" id="age" name="age">
            CREATE DATABASE medical_db;

USE medical_db;

CREATE TABLE patients (
    id INT AUTO_INCREMENT PRIMARY KEY,
    regNumber VARCHAR(50),
    nicNumber VARCHAR(50),
    date DATE,
    age INT,
    address VARCHAR(255),
    workingDiagnosis VARCHAR(255),
    treatment VARCHAR(255)
);
<?php
$servername = "localhost";
$username = "root"; // Replace with your database username
$password = ""; // Replace with your database password
$dbname = "medical_db";

// Create connection
$conn = new mysqli($servername, $username, $password, $dbname);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
?>
<form action="submit_patient.php" method="post">
    <!-- form fields as before -->
</form>

            <label for="address">Address:</label>
            <input type="text" id="address" name="address">
            
            <label for="workingDiagnosis">Working Diagnosis:</label>
            <input type="text" id="workingDiagnosis" name="workingDiagnosis">
            
            <label for="treatment">Treatment:</label>
            <input type="text" id="treatment" name="treatment">
            
            <button type="submit">Submit</button>
        </form>
    </div>
</div>

</body>
</html>
