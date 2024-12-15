<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday!</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background: #000;
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }

        .container {
            text-align: center;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
        }

        h1 {
            font-size: 3rem;
            margin: 10px 0;
            color: #ff6363;
        }

        h2 {
            font-size: 2rem;
            color: #ff9f43;
        }

        .message {
            margin: 20px 0;
            font-size: 1.2rem;
            color: #ddd;
        }

        .balloons {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: -1;
            overflow: hidden;
        }

        .balloon {
            position: absolute;
            bottom: -150px;
            width: 80px;
            height: 100px;
            background: red;
            border-radius: 50%;
            animation: float 7s ease-in-out infinite;
            box-shadow: inset -10px -10px 0 rgba(0, 0, 0, 0.2);
        }

        .balloon:nth-child(2) {
            background: blue;
            left: 20%;
            animation-duration: 8s;
        }

        .balloon:nth-child(3) {
            background: yellow;
            left: 40%;
            animation-duration: 6s;
        }

        .balloon:nth-child(4) {
            background: pink;
            left: 60%;
            animation-duration: 9s;
        }

        .balloon:nth-child(5) {
            background: green;
            left: 80%;
            animation-duration: 7.5s;
        }

        @keyframes float {
            0% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-300px);
            }

            100% {
                transform: translateY(0);
            }
        }

        .sky-crackers {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
            top: 0;
            left: 0;
            z-index: -2;
        }

        .cracker {
            position: absolute;
            width: 40px;
            height: 40px;
            background: radial-gradient(circle, yellow, orange, red);
            border-radius: 50%;
            opacity: 0;
            animation: explode 1.5s ease-out infinite;
            filter: brightness(2);
        }

        .cracker:nth-child(1) {
            left: 10%;
            top: 20%;
            background: radial-gradient(circle, yellow, orange, red);
            animation-delay: 0.5s;
        }
        .cracker:nth-child(2) {
            left: 30%;
            top: 40%;
            background: radial-gradient(circle, cyan, blue, navy);
            animation-delay: 1s;
        }
        .cracker:nth-child(3) {
            left: 50%;
            top: 10%;
            background: radial-gradient(circle, rgb(4, 236, 4), rgb(11, 106, 11), rgb(6, 65, 6));
            animation-delay: 1.5s;
        }
        .cracker:nth-child(4) {
            left: 70%;
            top: 30%;
            background: radial-gradient(circle, violet, purple, darkviolet);
            animation-delay: 2s;
        }
        .cracker:nth-child(5) {
            left: 90%;
            top: 50%;
            background: radial-gradient(circle, pink, hotpink, red);
            animation-delay: 2.5s;
        }
        .cracker:nth-child(6) {
            left: 20%;
            top: 70%;
            background: radial-gradient(circle, rgb(255, 102, 0), rgb(187, 187, 9), rgb(251, 215, 14));
            animation-delay: 1.2s;
        }
        .cracker:nth-child(7) {
            left: 80%;
            top: 80%;
            background: radial-gradient(circle, aqua, turquoise, teal);
            animation-delay: 1.8s;
        }

        @keyframes explode {
            0% {
                opacity: 1;
                transform: scale(0);
            }
            50% {
                opacity: 0.7;
                transform: scale(5);
            }
            100% {
                opacity: 0;
                transform: scale(8);
            }
        }
    </style>
</head>
<body>
    <div class="balloons">
        <div class="balloon"></div>
        <div class="balloon"></div>
        <div class="balloon"></div>
        <div class="balloon"></div>
        <div class="balloon"></div>
    </div>
    <div class="sky-crackers">
        <div class="cracker"></div>
        <div class="cracker"></div>
        <div class="cracker"></div>
        <div class="cracker"></div>
        <div class="cracker"></div>
        <div class="cracker"></div>
        <div class="cracker"></div>
    </div>
    <div class="container">
        <h1>Happy Birthday!</h1>
        <h2> ALU! </h2>
        <p class="message">Yo
Happy birthday, you absolute legend! 🎉 Another year of you being the shy, socially awkward genius we all tolerate (and secretly admire). Honestly, it sucks that I can’t be there to celebrate with you this year, but don’t think you’re off the hook! Just because we’re in different cities doesn’t mean you get to spend your birthday hiding in your room like a hermit.

Bro, it’s your day—ditch the shy guy routine, step out, and make some moves! Go meet some girls (and no, I don’t mean scrolling through Instagram). You’ve got the charm, the brains, and, well, you have me as your hype man, even from a distance. So, no excuses!

This year, I want you to forget all the awkwardness, embrace your inner alpha, and make the most of it. We’ll celebrate together properly when we meet, but until then, promise me you’ll at least do something exciting. And if not, just know I’ll roast you for it later.

Here’s to more laughs, crazy moments, and you finally stepping out of your comfort zone. Happy birthday, bro! I miss you, but that doesn’t mean I’ll stop teasing you.

Cheers,!</p>
    </div>
</body>
</html>
