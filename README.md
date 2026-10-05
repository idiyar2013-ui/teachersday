<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ұстазым, мерекеңізбен! 🌷</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            min-height: 100vh;
            font-family: Arial, sans-serif;
            overflow-x: hidden;
            background:
                radial-gradient(circle at 20% 20%, #fff3b0 0%, transparent 25%),
                radial-gradient(circle at 80% 30%, #ffd6e7 0%, transparent 30%),
                linear-gradient(135deg, #f7efe2, #fff8ed, #f5e1d2);
            color: #3d3028;
        }
        /* Анимация фоновых частиц */
        .particle {
            position: fixed;
            color: #d4a84f;
            font-size: 20px;
            animation: fall linear infinite;
            opacity: 0.7;
            z-index: 0;
        }
        @keyframes fall {
            0% {
                transform: translateY(-100px) rotate(0deg);
                opacity: 0;
            }
            20% {
                opacity: 0.8;
            }
            100% {
                transform: translateY(110vh) rotate(360deg);
                opacity: 0;
            }
        }
        .wrapper {
            position: relative;
            z-index: 2;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 40px 20px;
        }
        .card {
            width: 100%;
            max-width: 850px;
            padding: 55px 45px;
            text-align: center;
            background: rgba(255, 255, 255, 0.78);
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.9);
            border-radius: 35px;
            box-shadow:
                0 30px 80px rgba(100, 70, 40, 0.18),
                inset 0 0 40px rgba(255,255,255,0.5);
            animation: appear 1.2s ease;
        }
        @keyframes appear {
            from {
                opacity: 0;
                transform: translateY(40px) scale(0.95);
            }
            to {
                opacity: 1;
                transform: translateY(0) scale(1);
            }
        }
        .flowers {
            font-size: 58px;
            margin-bottom: 15px;
            animation: floating 3s ease-in-out infinite;
        }
        @keyframes floating {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
        .small-title {
            color: #b58a3a;
            letter-spacing: 4px;
            text-transform: uppercase;
            font-size: 14px;
            font-weight: bold;
        }
        h1 {
            margin: 15px 0;
            font-family: Georgia, serif;
            font-size: clamp(38px, 7vw, 68px);
            color: #9a7028;
            line-height: 1.1;
        }
        .subtitle {
            font-size: 22px;
            color: #66554a;
            margin-bottom: 35px;
        }
        .line {
            width: 100px;
            height: 3px;
            margin: 0 auto 30px;
            background: linear-gradient(90deg, transparent, #d4a84f, transparent);
        }
        .message {
            max-width: 680px;
            margin: auto;
            padding: 30px;
            background: rgba(255, 248, 235, 0.8);
            border-radius: 25px;
            border: 1px solid rgba(212, 168, 79, 0.25);
        }
        .message p {
            font-size: 19px;
            line-height: 1.8;
            margin-bottom: 15px;
        }
        .message p:last-child {
            margin-bottom: 0;
        }
        .highlight {
            color: #a57929;
            font-weight: bold;
        }
        button {
            margin-top: 30px;
            padding: 16px 35px;
            border: none;
            border-radius: 50px;
            background: linear-gradient(135deg, #d4a84f, #b9862f);
            color: white;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            box-shadow: 0 10px 25px rgba(170, 120, 40, 0.3);
            transition: 0.3s;
        }
        button:hover {
            transform: translateY(-4px) scale(1.03);
            box-shadow: 0 15px 30px rgba(170, 120, 40, 0.4);
        }
        button:active {
            transform: scale(0.96);
        }
        #surprise {
            display: none;
            margin-top: 30px;
            animation: surprise 0.7s ease;
        }
        @keyframes surprise {
            from {
                opacity: 0;
                transform: scale(0.7);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        #surprise h2 {
            color: #a57929;
            font-family: Georgia, serif;
            font-size: 30px;
            margin-bottom: 10px;
        }
        #surprise p {
            font-size: 18px;
            color: #66554a;
        }
        footer {
            margin-top: 35px;
            color: #8c7b6d;
            font-size: 14px;
        }
        @media (max-width: 600px) {
            .card {
                padding: 40px 20px;
            }
            .message {
                padding: 22px;
            }
            .message p {
                font-size: 17px;
            }
            .subtitle {
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <!-- Фоновые частицы -->
    <div class="particle" style="left:5%; animation-duration:9s;">✦</div>
    <div class="particle" style="left:15%; animation-duration:12s;">✧</div>
    <div class="particle" style="left:28%; animation-duration:10s;">✦</div>
    <div class="particle" style="left:42%; animation-duration:14s;">✧</div>
    <div class="particle" style="left:58%; animation-duration:11s;">✦</div>
    <div class="particle" style="left:72%; animation-duration:13s;">✧</div>
    <div class="particle" style="left:88%; animation-duration:9s;">✦</div>
    <main class="wrapper">
        <section class="card">
            <div class="flowers">
                🌷 ✨ 🌷
            </div>
            <div class="small-title">
                Ұстаздар күні
            </div>
            <h1>
                Ұстазым,<br>
                мерекеңізбен!
            </h1>
            <p class="subtitle">
                Білім бергеніңіз үшін мың алғыс! 🤍
            </p>
            <div class="line"></div>
            <div class="message">
                <p>
                    <span class="highlight">Құрметті ұстаз!</span>
                </p>
                <p>
                    Сізді Ұстаздар күнімен шын жүректен
                    құттықтаймыз! 🌷
                </p>
                <p>
                    Сізге зор денсаулық, отбасылық бақыт,
                    шығармашылық табыс және сарқылмас
                    күш-қуат тілейміз.
                </p>
                <p>
                    Бізге білім беріп қана қоймай,
                    әрқашан қолдау көрсетіп,
                    дұрыс жол сілтеп жүргеніңіз үшін
                    үлкен рақмет!
                </p>
                <p>
                    Сіздің әрбір сабағыңыз, әрбір ақылыңыз
                    және бізге деген сеніміңіз біз үшін
                    өте маңызды. ❤️
                </p>
                <p>
                    <span class="highlight">
                        Еңбегіңіз әрдайым бағаланып,
                        шәкірттеріңіздің жетістігі
                        сізге қуаныш сыйласын!
                    </span>
                </p>
            </div>
            <button onclick="showSurprise()">
                🎁 Арнайы сыйлық
            </button>
            <div id="surprise">
                <h2>
                    Сіз — керемет ұстазсыз! 🌟
                </h2>
                <p>
                    Сізге үлкен рақмет! ❤️
                </p>
                <div style="font-size:40px; margin-top:15px;">
                    🌷 📚 ✨ 💐 ❤️
                </div>
            </div>
            <footer>
                Ізгі ниетпен, шәкірттеріңізден 💐
            </footer>
        </section>
    </main>
    <script>
        function showSurprise() {
            const surprise =
                document.getElementById("surprise");
            surprise.style.display = "block";
            // Небольшой салют из символов
            for (let i = 0; i < 20; i++) {
                const star = document.createElement("div");
                star.innerHTML = "✦";
                star.style.position = "fixed";
                star.style.left = "50%";
                star.style.top = "50%";
                star.style.fontSize = "25px";
                star.style.color = "#d4a84f";
                star.style.pointerEvents = "none";
                star.style.zIndex = "999";
                document.body.appendChild(star);
                const angle = Math.random() * Math.PI * 2;
                const distance = 100 + Math.random() * 250;
                const x = Math.cos(angle) * distance;
                const y = Math.sin(angle) * distance;
                star.animate(
                    [
                        {
                            transform: "translate(-50%, -50%) scale(0)",
                            opacity: 1
                        },
                        {
                            transform:
                                `translate(${x}px, ${y}px) scale(1.5)`,
                            opacity: 0
                        }
                    ],
                    {
                        duration: 1000,
                        easing: "ease-out"
                    }
                );
                setTimeout(() => {
                    star.remove();
                }, 1000);
            }
        }
    </script>
</body>
</html>
