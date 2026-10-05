<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Ұстаздар күні</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            min-height: 100vh;
            background: linear-gradient(135deg, #f8efe0, #f7d9df);
            color: #3d3028;
            overflow-x: hidden;
        }

        /* Фон */
        .background {
            position: fixed;
            inset: 0;
            overflow: hidden;
            z-index: 0;
        }

        .circle {
            position: absolute;
            border-radius: 50%;
            filter: blur(2px);
            opacity: 0.35;
        }

        .circle1 {
            width: 350px;
            height: 350px;
            background: #e8b96a;
            top: -120px;
            left: -100px;
        }

        .circle2 {
            width: 400px;
            height: 400px;
            background: #e99aaa;
            bottom: -180px;
            right: -100px;
        }

        /* Основная карточка */
        .container {
            position: relative;
            z-index: 1;

            width: 90%;
            max-width: 850px;

            margin: 60px auto;
            padding: 60px 45px;

            background: rgba(255, 255, 255, 0.9);
            border-radius: 30px;

            box-shadow: 0 25px 70px rgba(70, 45, 30, 0.18);

            text-align: center;

            animation: appear 1s ease;
        }

        @keyframes appear {
            from {
                opacity: 0;
                transform: translateY(35px);
            }

            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .top {
            color: #b38332;
            font-size: 14px;
            font-weight: bold;
            letter-spacing: 4px;
            text-transform: uppercase;
        }

        h1 {
            margin-top: 18px;

            font-family: Georgia, serif;

            font-size: clamp(42px, 8vw, 70px);

            line-height: 1.05;

            color: #a87928;
        }

        .subtitle {
            margin-top: 20px;

            font-size: 21px;

            color: #6d5a4d;
        }

        .line {
            width: 100px;
            height: 3px;

            margin: 30px auto;

            background: #d0a04a;
        }

        /* Текст */
        .message {
            background: #fff8ec;

            border-radius: 22px;

            padding: 35px;

            border: 1px solid #f0dfbd;
        }

        .message h2 {
            margin-bottom: 20px;

            font-family: Georgia, serif;

            color: #a87928;

            font-size: 30px;
        }

        .message p {
            font-size: 18px;
            line-height: 1.8;

            margin-bottom: 16px;
        }

        .message p:last-child {
            margin-bottom: 0;
        }

        /* Кнопка */
        button {
            margin-top: 30px;

            padding: 16px 35px;

            border: none;
            border-radius: 50px;

            background: #b98936;

            color: white;

            font-size: 18px;
            font-weight: bold;

            cursor: pointer;

            transition: 0.3s;

            box-shadow: 0 10px 25px rgba(150, 100, 30, 0.25);
        }

        button:hover {
            transform: translateY(-4px);

            background: #9e752d;

            box-shadow: 0 15px 30px rgba(150, 100, 30, 0.3);
        }

        button:active {
            transform: scale(0.96);
        }

        /* Сюрприз */
        #surprise {
            display: none;

            margin-top: 30px;

            padding: 25px;

            border-radius: 20px;

            background: #f9e6ea;

            animation: popup 0.5s ease;
        }

        #surprise h2 {
            font-family: Georgia, serif;

            color: #a04d61;

            margin-bottom: 10px;
        }

        #surprise p {
            font-size: 18px;
        }

        @keyframes popup {
            from {
                opacity: 0;
                transform: scale(0.8);
            }

            to {
                opacity: 1;
                transform: scale(1);
            }
        }

        footer {
            margin-top: 35px;

            color: #8b7769;

            font-size: 14px;
        }

        /* Телефон */
        @media (max-width: 600px) {

            .container {
                padding: 40px 20px;
                margin: 25px auto;
            }

            .message {
                padding: 25px 18px;
            }

            .message p {
                font-size: 16px;
            }

            .subtitle {
                font-size: 18px;
            }
        }
    </style>
</head>

<body>

    <div class="background">
        <div class="circle circle1"></div>
        <div class="circle circle2"></div>
    </div>

    <div class="container">

        <div class="top">
            Ұстаздар күні
        </div>

        <h1>
            Ұстазым,<br>
            мерекеңізбен!
        </h1>

        <p class="subtitle">
            Сіздің еңбегіңізге шын жүректен алғыс білдіреміз
        </p>

        <div class="line"></div>

        <div class="message">

            <h2>Құрметті ұстаз!</h2>

            <p>
                Сізді Ұстаздар күнімен шын жүректен құттықтаймыз!
            </p>

            <p>
                Сізге зор денсаулық, мол бақыт,
                отбасылық береке және шығармашылық
                табыс тілейміз.
            </p>

            <p>
                Бізге білім беріп, әрқашан қолдау көрсетіп,
                дұрыс жол сілтегеніңіз үшін үлкен рақмет!
            </p>

            <p>
                Сіздің әрбір сабағыңыз бен ақылыңыз
                біз үшін өте маңызды.
            </p>

            <p>
                Шәкірттеріңіздің жетістігі сізге әрдайым
                қуаныш сыйласын!
            </p>

        </div>

        <button onclick="showMessage()">
            Арнайы құттықтауды ашу
        </button>

        <div id="surprise">

            <h2>
                Сізге үлкен рақмет!
            </h2>

            <p>
                Сіз — бізге білім беретін ғана емес,
                болашаққа жол көрсететін жансыз.
            </p>

        </div>

        <footer>
            Ізгі ниетпен, шәкірттеріңізден
        </footer>

    </div>

    <script>

        function showMessage() {

            const message = document.getElementById("surprise");

            message.style.display = "block";

        }

    </script>

</body>
</html>
