<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love in the Air</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to bottom right, #FFAFBD, #ffc3a0);
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            position: relative;
            color: #fff;
        }

        .container {
            text-align: center;
            z-index: 2;
            animation: fadeIn 2s ease-in-out;
        }

        h1 {
            font-size: 4rem;
            margin: 0;
            font-weight: bold;
            color: #ffedda;
            text-shadow: 0 0 20px rgba(255, 255, 255, 0.6);
        }

        p {
            font-size: 1.5rem;
            margin-top: 1rem;
            color: #fef9f8;
            font-style: italic;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.4);
        }

        .btn {
            margin-top: 2rem;
            padding: 1rem 2.5rem;
            font-size: 1.5rem;
            background: #ff6f61;
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, background 0.5s ease;
        }

        .btn:hover {
            background: #ff847c;
            transform: translateY(-5px);
        }

        .btn:active {
            background: #f86c70;
            transform: translateY(2px);
        }

        .hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            overflow: hidden;
        }

        .heart {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff6f61;
            transform: rotate(45deg);
            animation: float 10s linear infinite;
        }

        .heart::before,
        .heart::after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: #ff6f61;
            border-radius: 50%;
        }

        .heart::before {
            top: -10px;
            left: 0;
        }

        .heart::after {
            left: 10px;
            top: 0;
        }

        @keyframes float {
            0% {
                transform: translateY(0) rotate(45deg);
            }
            100% {
                transform: translateY(-100vh) rotate(45deg);
            }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.8); }
            to { opacity: 1; transform: scale(1); }
        }

        /* Random heart positions */
        .heart:nth-child(2) { animation-duration: 8s; left: 10%; animation-delay: 1s; }
        .heart:nth-child(3) { animation-duration: 12s; left: 20%; animation-delay: 2s; }
        .heart:nth-child(4) { animation-duration: 10s; left: 30%; animation-delay: 3s; }
        .heart:nth-child(5) { animation-duration: 14s; left: 40%; animation-delay: 4s; }
        .heart:nth-child(6) { animation-duration: 9s; left: 50%; animation-delay: 5s; }
        .heart:nth-child(7) { animation-duration: 13s; left: 60%; animation-delay: 6s; }
        .heart:nth-child(8) { animation-duration: 11s; left: 70%; animation-delay: 7s; }
        .heart:nth-child(9) { animation-duration: 15s; left: 80%; animation-delay: 8s; }
        .heart:nth-child(10) { animation-duration: 12s; left: 90%; animation-delay: 9s; }
    </style>
</head>
<body>
    <div class="container">
        <h1>Love is in the Air</h1>
        <p>Tu amor esta en el aire</p>
        <button class="btn" onclick="burstHeart()">Siente a tu amor!!!</button>
    </div>

    <div class="hearts" id="hearts"></div>

    <script>
        function burstHeart() {
            // Generate burst of hearts
            for (let i = 0; i < 20; i++) {
                createBurstingHeart();
            }
        }

        function createBurstingHeart() {
            const heartsContainer = document.getElementById('hearts');
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.top = Math.random() * 100 + 'vh';
            heart.style.width = Math.random() * 20 + 10 + 'px';
            heart.style.height = heart.style.width;
            heart.style.animationDuration = Math.random() * 2 + 3 + 's';

            heartsContainer.appendChild(heart);

            // Remove heart after animation ends
            setTimeout(() => {
                heart.remove();
            }, 5000);
        }
    </script>
</body>
</html>
