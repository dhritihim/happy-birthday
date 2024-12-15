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
            padding: 20px;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
            max-width: 90%;
        }

        h1 {
            font-size: 2.5rem;
            margin: 10px 0;
            color: #ff6363;
        }

        h2 {
            font-size: 1.8rem;
            color: #ff9f43;
        }

        .message {
            margin: 20px 0;
            font-size: 1rem;
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
            width: 60px;
            height: 80px;
            background: red;
            border-radius: 50%;
            animation: float 7s ease-in-out infinite;
            box-shadow: inset -10px -10px 0 rgba(0, 0, 0, 0.2);
        }

        .balloon:nth-child(2) {
            background: blue;
            left: 15%;
            animation-duration: 8s;
        }

        .balloon:nth-child(3) {
            background: yellow;
            left: 35%;
            animation-duration: 6s;
        }

        .balloon:nth-child(4) {
            background: pink;
            left: 55%;
            animation-duration: 9s;
        }

        .balloon:nth-child(5) {
            background: green;
            left: 75%;
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
            width: 30px;
            height: 30px;
            background: radial-gradient(circle, yellow, orange, red);
            border-radius: 50%;
            opacity: 0;
            animation: explode 1.5s ease-out infinite;
            filter: brightness(2);
        }

        .cracker:nth-child(1) { left: 5%; top: 10%; animation-delay: 0.5s; }
        .cracker:nth-child(2) { left: 25%; top: 30%; animation-delay: 1s; }
        .cracker:nth-child(3) { left: 45%; top: 20%; animation-delay: 1.5s; }
        .cracker:nth-child(4) { left: 65%; top: 35%; animation-delay: 2s; }
        .cracker:nth-child(5) { left: 85%; top: 45%; animation-delay: 2.5s; }
        .cracker:nth-child(6) { left: 15%; top: 70%; animation-delay: 1.2s; }
        .cracker:nth-child(7) { left: 70%; top: 75%; animation-delay: 1.8s; }

        @keyframes explode {
            0% {
                opacity: 1;
                transform: scale(0);
            }
            50% {
                opacity: 0.7;
                transform: scale(3);
            }
            100% {
                opacity: 0;
                transform: scale(5);
            }
        }

        /* Media Queries for Responsive Design */
        @media (max-width: 768px) {
            h1 {
                font-size: 1.8rem;
            }

            h2 {
                font-size: 1.3rem;
            }

            .message {
                font-size: 0.9rem;
            }

            .balloon {
                width: 40px;
                height: 60px;
            }

            .cracker {
                width: 20px;
                height: 20px;
            }

            .container {
                padding: 10px;
                max-width: 95%;
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 1.5rem;
            }

            h2 {
                font-size: 1rem;
            }

            .message {
                font-size: 0.8rem;
            }

            .balloon {
                width: 30px;
                height: 50px;
            }

            .cracker {
                width: 15px;
                height: 15px;
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
        <h2>ALU ! </h2>
        <p class="message">Yo<br>
            Happy birthday, you absolute legend! 🎉 Another year of you being the shy, socially awkward genius we all tolerate (and secretly admire). Honestly, it sucks that I can't be there to celebrate with you this year, but don't think you're off the hook! Just because we're in different cities doesn't mean you get to spend your birthday hiding in your room like a hermit.<br>
            Bro, it's your day ditch the shy guy routine, step out, and make some moves! You've got the charm, the brains, and, well, you have me as your hype man. Cheers! 🎉</p>
    </div>
</body>
</html>
