<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mini Game</title>
    <style>
        body { text-align: center; font-family: Arial, sans-serif; }
        canvas { background: #ddd; display: block; margin: 20px auto; }
        button { font-size: 20px; padding: 10px 20px; margin-top: 20px; }
        .level-bar { margin: 10px auto; width: 80%; height: 20px; background: lightgray; position: relative; }
        .level-progress { height: 100%; width: 0%; background: green; transition: width 0.3s; }
    </style>
</head>
<body>
    <h1>Попробуй остановить черный круг в красном!</h1>
    <div class="level-bar">
        <div class="level-progress"></div>
    </div>
    <canvas id="gameCanvas" width="400" height="100"></canvas>
    <button onclick="stopCircle()">СТОП</button>
    <p id="result"></p>

    <script>
        const canvas = document.getElementById("gameCanvas");
        const ctx = canvas.getContext("2d");
        let level = 1;
        let x = 200;
        let speed = 3;
        let moving = true;
        const redZoneStart = canvas.width / 2 - 20;
        const redZoneEnd = canvas.width / 2 + 20;

        function draw() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            
            // Красный круг (целевая область)
            ctx.fillStyle = "red";
            ctx.beginPath();
            ctx.arc(canvas.width / 2, canvas.height / 2, 25, 0, Math.PI * 2);
            ctx.fill();
            
            // Черный движущийся круг
            ctx.fillStyle = "black";
            ctx.beginPath();
            ctx.arc(x, canvas.height / 2, 15, 0, Math.PI * 2);
            ctx.fill();
            
            if (moving) {
                x += speed;
                if (x > canvas.width - 20 || x < 20) speed = -speed;
                requestAnimationFrame(draw);
            }
        }

        function stopCircle() {
            moving = false;
            if (x >= redZoneStart && x <= redZoneEnd) {
                if (level < 8) {
                    level++;
                    document.querySelector(".level-progress").style.width = (level * 12.5) + "%";
                    moving = true;
                    draw();
                } else {
                    document.getElementById("result").innerText = "Ты прошел все уровни!";
                    setTimeout(() => {
                        window.Telegram.WebApp.close();
                    }, 2000);
                }
            } else {
                document.getElementById("result").innerText = "Промах! Попробуй снова.";
                moving = true;
                draw();
            }
        }

        draw();
    </script>
</body>
</html>
