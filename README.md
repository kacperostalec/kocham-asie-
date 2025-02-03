<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kocham Cię Asia</title>
    <style>
        body {
            background-color: red;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            color: black;
            font-size: 48px;
            font-weight: bold;
            text-align: center;
            animation: fadeIn 3s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .heart-button {
            margin-top: 20px;
            width: 60px;
            height: 60px;
            background-color: black;
            position: relative;
            transform: rotate(-45deg);
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
        }
        .heart-button::before,
        .heart-button::after {
            content: "";
            width: 60px;
            height: 60px;
            background-color: black;
            border-radius: 50%;
            position: absolute;
        }
        .heart-button::before {
            top: -30px;
            left: 0;
        }
        .heart-button::after {
            left: 30px;
            top: 0;
        }
        .heart-button:hover {
            transform: scale(1.1) rotate(-45deg);
        }
    </style>
</head>
<body>
    Kocham Cię Asia
    <div class="heart-button" onclick="window.location.href='druga_strona.html'"></div>
</body>
</html>
