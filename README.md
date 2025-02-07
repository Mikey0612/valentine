# valentine
yes or no 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffe6e6;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        h1 {
            color: #ff4d4d;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #cccccc;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Will you be my Valentine Nigga? ❤️</h1>
        <div class="buttons">
            <button class="yes" onclick="sayYes()">Yes</button>
            <button class="no" onmouseover="moveButton(this)">No</button>
        </div>
        <p id="message"></p>
    </div>

    <script>
        function sayYes() {
            document.getElementById('message').innerText = "Yay! ❤️ Can't wait!";
        }
        
        function moveButton(button) {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.position = "absolute";
            button.style.left = `${x}px`;
            button.style.top = `${y}px`;
        }
    </script>
</body>
</html>
