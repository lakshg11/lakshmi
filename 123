<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BMI Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            max-width: 300px;
            width: 100%;
        }

        h1 {
            text-align: center;
            margin-bottom: 20px;
        }

        input[type="number"] {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            width: 100%;
            padding: 10px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        button:hover {
            background-color: #218838;
        }

        .result {
            text-align: center;
            margin-top: 20px;
            font-size: 1.2em;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>BMI Calculator</h1>
        <input type="number" id="weight" placeholder="Weight (kg)">
        <input type="number" id="height" placeholder="Height (cm)">
        <button onclick="calculateBMI()">Calculate</button>
        <div class="result" id="result"></div>
    </div>
    <script>
        function calculateBMI() {
            let weight = document.getElementById('weight').value;
            let height = document.getElementById('height').value;
            
            if (weight === '' || height === '') {
                alert('Please enter valid weight and height!');
                return;
            }

            height = height / 100; // converting height from cm to meters
            let bmi = weight / (height * height);
            bmi = bmi.toFixed(2);

            let resultText = 'Your BMI is ' + bmi;

            if (bmi < 18.5) {
                resultText += ' (Underweight)';
            } else if (bmi >= 18.5 && bmi < 24.9) {
                resultText += ' (Normal weight)';
            } else if (bmi >= 25 && bmi < 29.9) {
                resultText += ' (Overweight)';
            } else {
                resultText += ' (Obesity)';
            }

            document.getElementById('result').innerText = resultText;
        }
    </script>
</body>
</html>
