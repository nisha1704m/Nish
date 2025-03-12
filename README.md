<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML, CSS, and JavaScript Example</title>
    <style>
        /* CSS Styles */
        /* Reset some basic styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body styles */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            text-align: center;
            padding: 50px;
            transition: background-color 0.3s ease;
        }

        /* Header styling */
        header {
            background-color: #4CAF50;
            padding: 10px;
            color: white;
            border-radius: 5px;
        }

        h1 {
            font-size: 2.5em;
        }

        /* Button styling */
        .cta-button {
            padding: 15px 25px;
            background-color: #008CBA;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1.2em;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .cta-button:hover {
            background-color: #005f73;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Interactive Webpage</h1>
    </header>
    <main>
        <p>This is a simple webpage with HTML, CSS, and JavaScript.</p>
        <button class="cta-button" onclick="changeBackgroundColor()">Click to Change Background Color</button>
    </main>

    <script>
        // JavaScript function to change the background color
        function changeBackgroundColor() {
            // Array of colors to choose from
            const colors = ["#f4f4f4", "#FFDDC1", "#D4E157", "#81C784", "#FFEB3B", "#FF5722"];
            // Randomly pick a color from the array
            const randomColor = colors[Math.floor(Math.random() * colors.length)];
            // Set the background color to the randomly selected color
            document.body.style.backgroundColor = randomColor;
        }
    </script>
</body>
</html>
