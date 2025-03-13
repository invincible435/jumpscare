<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Troll Site</title>
    <style>
        body {
            text-align: center;
            padding: 50px;
            font-family: Arial, sans-serif;
            background-color: black;
            color: white;
        }
        #scary-img {
            display: none;
            width: 100vw;
            height: 100vh;
            position: fixed;
            top: 0;
            left: 0;
            z-index: 9999;
        }
    </style>
</head>
<body>
    <h1>Bu siteye devam etmek için "Accept"e tıklayın</h1>
    <button id="accept-btn">Accept</button>

    <img id="scary-img" src="scary.jpg" alt="Jumpscare">
    <audio id="scary-audio" src="scream.mp3"></audio>

    <script>
        document.getElementById("accept-btn").addEventListener("click", function() {
            document.getElementById("scary-img").style.display = "block";
            var audio = document.getElementById("scary-audio");
            audio.play();
        });
    </script>
</body>
</html>
