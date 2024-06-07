# birthday-greeting-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Chine</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: url('https://i.imgur.com/1bE7bTG.jpg') no-repeat center center fixed;
            background-size: cover;
            font-family: 'Comic Sans MS', cursive, sans-serif;
            overflow: hidden;
        }
        .card {
            text-align: center;
            padding: 50px;
            background: rgba(255, 255, 255, 0.8);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            border-radius: 15px;
            opacity: 0;
            animation: fadeIn 2s forwards, scaleUp 1s 2s forwards;
        }
        .card h1 {
            font-size: 3em;
            color: #ff6347;
            animation: textGlow 1s infinite;
        }
        .card p {
            font-size: 1.5em;
            color: #333;
        }
        .tulips {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }
        .tulip {
            position: absolute;
            width: 50px;
            height: 100px;
            background-color: #ff6347;
            border-radius: 50% 50% 0 0;
            transform: rotate(45deg);
            animation: float 6s ease-in-out infinite, moveTulips 10s linear infinite;
        }
        .tulip::before {
            content: '';
            position: absolute;
            width: 100%;
            height: 100%;
            background-color: inherit;
            border-radius: 50%;
            transform: rotate(-90deg);
        }
        .tulip:nth-child(2) {
            background-color: #ffdd57;
            left: 20%;
            animation-duration: 7s, 12s;
        }
        .tulip:nth-child(3) {
            background-color: #c1e1c1;
            left: 40%;
            animation-duration: 5s, 11s;
        }
        .tulip:nth-child(4) {
            background-color: #87ceeb;
            left: 60%;
            animation-duration: 6.5s, 13s;
        }
        .tulip:nth-child(5) {
            background-color: #d94f70;
            left: 80%;
            animation-duration: 6s, 14s;
        }
        @keyframes float {
            0% {
                transform: translateY(0) rotate(45deg);
            }
            50% {
                transform: translateY(-20px) rotate(45deg);
            }
            100% {
                transform: translateY(0) rotate(45deg);
            }
        }
        @keyframes moveTulips {
            0% {
                top: 100%;
                left: 0;
                transform: translateX(0);
            }
            100% {
                top: -10%;
                left: 100%;
                transform: translateX(-100%);
            }
        }
        @keyframes fadeIn {
            to {
                opacity: 1;
            }
        }
        @keyframes scaleUp {
            to {
                transform: scale(1.1);
            }
        }
        @keyframes textGlow {
            0%, 100% {
                text-shadow: 0 0 5px #ff6347, 0 0 10px #ff6347, 0 0 15px #ff6347, 0 0 20px #ff6347, 0 0 25px #ff6347, 0 0 30px #ff6347, 0 0 35px #ff6347;
            }
            50% {
                text-shadow: 0 0 10px #ff6347, 0 0 20px #ff6347, 0 0 30px #ff6347, 0 0 40px #ff6347, 0 0 50px #ff6347, 0 0 60px #ff6347, 0 0 70px #ff6347;
            }
        }
    </style>
</head>
<body>
    <div class="tulips">
        <div class="tulip"></div>
        <div class="tulip"></div>
        <div class="tulip"></div>
        <div class="tulip"></div>
        <div class="tulip"></div>
    </div>
    <div class="card">
        <h1>Happy Birthday, Chine!</h1>
        <p>June 9th</p>
    </div>
</body>
</html>
