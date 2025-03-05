<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tournament Registration</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: url('https://wallpaperaccess.com/full/1260281.jpg') no-repeat center center/cover;
            font-family: Arial, sans-serif;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .container {
            background: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0,0,0,0.5);
            max-width: 900px;
            width: 100%;
            text-align: center;
        }
        h1 {
            margin-bottom: 20px;
            font-size: 2.5rem;
            color: #ffcc00;
        }
        .columns {
            display: flex;
            justify-content: space-between;
            gap: 20px;
        }
        .column {
            flex: 1;
            background: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 8px;
            border: 2px solid #ffcc00;
        }
        h2 {
            font-size: 1.8rem;
            color: #ffcc00;
            margin-bottom: 10px;
        }
        .info {
            text-align: left;
            font-size: 1rem;
            margin-bottom: 15px;
        }
        input {
            width: 90%;
            padding: 10px;
            margin: 5px 0;
            border: none;
            border-radius: 5px;
        }
        .register-btn {
            background: #ffcc00;
            color: black;
            border: none;
            padding: 12px 25px;
            font-size: 1.2rem;
            cursor: pointer;
            border-radius: 5px;
            transition: background 0.3s;
        }
        .register-btn:hover {
            background: #ffaa00;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>TOURNAMENT REGISTRATION</h1>
    <div class="columns">
        <!-- Solo Column -->
        <div class="column">
            <h2>SOLO</h2>
            <div class="info">
                Entry Fee: 150 Rupees<br>
                1. Booyah Prize: 1500 Rupees<br>
                2. 2nd Place Prize: 1000 Rupees<br>
                3. 3rd Place Prize: 500 Rupees<br>
            </div>
            <input type="text" placeholder="Player Name" id="soloName"><br>
            <input type="text" placeholder="Player ID" id="soloID"><br>
            <input type="text" placeholder="Player Number" id="soloNumber"><br>
        </div>

        <!-- Squad Column -->
        <div class="column">
            <h2>SQUAD</h2>
            <div class="info">
                Entry Fee: 1000 Rupees<br>
                1. Booyah Prize: 5000 Rupees & 1 Weekly<br>
                2. Per Kill: 40 Rupees<br>
            </div>
            <input type="text" placeholder="Team Leader Name" id="squadName"><br>
            <input type="text" placeholder="Team ID" id="squadID"><br>
            <input type="text" placeholder="Contact Number" id="squadNumber"><br>
        </div>
    </div>
    <br>
    <button class="register-btn" onclick="redirectToCongratulations()">REGISTER</button>
</div>

<script>
    function redirectToCongratulations() {
        // Here you can also capture form data if needed (optional)
        const soloName = document.getElementById('soloName').value;
        const soloID = document.getElementById('soloID').value;
        const soloNumber = document.getElementById('soloNumber').value;

        const squadName = document.getElementById('squadName').value;
        const squadID = document.getElementById('squadID').value;
        const squadNumber = document.getElementById('squadNumber').value;

        // Just an alert to show (optional - remove if you want)
        console.log(`Solo: ${soloName}, ${soloID}, ${soloNumber}`);
        console.log(`Squad: ${squadName}, ${squadID}, ${squadNumber}`);

        // Redirect to Congratulations Page (update path if needed)
        window.location.href = "file:///C:/Users/91790/Desktop/Website/conguralation.html";
    }
</script>

</body>
</html>
