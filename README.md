<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>❤️❤️</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Reem+Kufi+Ink:wght@700&display=swap');
        
        body {
            background-color: #ffebee;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            overflow: hidden;
        }
        
        .heart-container {
            position: relative;
            width: 90vmin;
            height: 90vmin;
            max-width: 800px;
            max-height: 800px;
        }
        
        .heart {
            position: absolute;
            width: 100%;
            height: 100%;
            animation: heartbeat 2s infinite;
            filter: drop-shadow(0 0 25px rgba(255, 0, 0, 0.8));
        }
        
        .heart:before, .heart:after {
            position: absolute;
            content: "";
            left: 50%;
            top: 0;
            width: 50%;
            height: 85%;
            background: linear-gradient(to bottom, #ff0000, #ff3333);
            border-radius: 50% 50% 0 0;
            transform: rotate(-45deg);
            transform-origin: 0 100%;
        }
        
        .heart:after {
            left: 0;
            transform: rotate(45deg);
            transform-origin: 100% 100%;
        }
        
        .text {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            font-size: 10vmin;
            font-weight: 700;
            font-family: 'Reem Kufi Ink', sans-serif;
            text-shadow: 
                0 0 10px #ff0000,
                0 0 20px #ff0000,
                0 0 30px #ff0000;
            z-index: 10;
            width: 100%;
            text-align: center;
            padding-bottom: 10%;
        }
        
        @keyframes heartbeat {
            0% { transform: scale(1); }
            30% { transform: scale(1.05); }
            50% { transform: scale(1); }
            70% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
    </style>
</head>
<body>
    <div class="heart-container">
        <div class="heart"></div>
        <div class="text">دميانه</div>
    </div>

    <script>
        const heart = document.querySelector('.heart');
        heart.addEventListener('click', function() {
            this.style.filter = 'drop-shadow(0 0 35px rgba(255, 0, 0, 0.9)) brightness(1.3)';
            setTimeout(() => {
                this.style.filter = 'drop-shadow(0 0 25px rgba(255, 0, 0, 0.8))';
            }, 300);
        });
    </script>
</body>
</html>
