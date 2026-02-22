<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <title>X0XR00T NEON BYPASS</title>
    <style>
        body {
            background-color: #050505;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            overflow: hidden;
        }

        /* De 'Restrictie Bypass' Container */
        .neon-container {
            position: relative;
            padding: 40px;
            border: 4px solid #00ff9c;
            border-radius: 10px;
            background: rgba(0, 0, 0, 0.8);
            
            /* De truc: gestapelde filters voor maximale glow-intensiteit */
            filter: drop-shadow(0 0 10px #00ff9c) 
                    drop-shadow(0 0 20px #00ff9c) 
                    drop-shadow(0 0 40px #ff0000);
            
            animation: flicker 1.5s infinite alternate;
        }

        .neon-text {
            font-family: 'Courier New', monospace;
            font-size: 3rem;
            font-weight: bold;
            color: #fff;
            text-align: center;
            text-transform: uppercase;
            /* Text-specific bypass glow */
            text-shadow: 0 0 5px #fff, 
                         0 0 10px #00ff9c, 
                         0 0 20px #00ff9c, 
                         0 0 40px #00ff9c;
        }

        /* Animatie voor de realistische 'vibrerende' terminal look */
        @keyframes flicker {
            0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
                opacity: 1;
                filter: drop-shadow(0 0 10px #00ff9c) drop-shadow(0 0 30px #ff0000);
            }
            20%, 24%, 55% {
                opacity: 0.8;
                filter: none;
            }
        }
    </style>
</head>
<body>

    <div class="neon-container">
        <div class="neon-text">RESTRICTION BYPASS<br>x0xr00t</div>
    </div>

</body>
</html>
