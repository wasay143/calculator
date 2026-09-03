<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Interest Calculator</title>
</head>
<body>

    <h1>Simple Interest Calculator</h1>

    <label>Principal Amount:</label>
    <input type="number" id="principal">

    <br><br>

    <label>Rate of Interest (%):</label>
    <input type="number" id="rate">

    <br><br>

    <label>Time (Years):</label>
    <input type="number" id="time">

    <br><br>

    <button onclick="calculateInterest()">Calculate</button>

    <h2 id="result"></h2>

    <script>
        function calculateInterest() {

            let principal = document.getElementById("principal").value;
            let rate = document.getElementById("rate").value;
            let time = document.getElementById("time").value;

            let simpleInterest = (principal * rate * time) / 100;

            let totalAmount = Number(principal) + simpleInterest;

            document.getElementById("result").innerHTML =
                "Simple Interest: " + simpleInterest +
                "<br>Total Amount: " + totalAmount;
        }
    </script>

</body>
</html>
```
