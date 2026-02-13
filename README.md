<!DOCTYPE html>
<html>
<head>
    <title>Be My Valentine 💖</title>

    <style>
        body {
            margin: 0;
            padding: 0;
            background: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
        }

        .container {
            text-align: center;
            position: relative;
            width: 350px;
        }

        img {
            width: 200px;
            margin-bottom: 20px;
        }

        h1 {
            color: #ff4d6d;
        }

        .buttons {
            margin-top: 20px;
            display: flex;
            justify-content: center;
            gap: 20px;
            position: relative;
            height: 60px;
        }

        button {
            padding: 12px 30px;
            font-size: 18px;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            color: white;
        }

        #yesBtn {
            background-color: green;
        }

        #noBtn {
            background-color: red;
            position: absolute;
            right: 0;
        }

        #sweetPage {
            display: none;
        }
    </style>
</head>

<body>

<div class="container">

    <!-- First Page Content -->
    <div id="questionPage">

        <h1>Will you be my Valentine? 💌</h1>
        <p>Think carefully 🥺</p>

        <div class="buttons">
            <button id="yesBtn" onclick="showSweet()">Yes 💚</button>
            <button id="noBtn" onclick="moveNo()">No ❤️</button>
        </div>
    </div>

    <!-- Sweet Page Content -->
    <div id="sweetPage">
        <h1>Yayyyy! 💕</h1>
        <p>I Know!!!🥰</p>
        <p>Happy Valentine's Day Mama💘</p>
    </div>

</div>

<script>
    function showSweet() {
        document.getElementById("questionPage").style.display = "none";
        document.getElementById("sweetPage").style.display = "block";
    }

    function moveNo() {
        var no = document.getElementById("noBtn");
        no.style.top = Math.random() * 40 + "px";
        no.style.left = Math.random() * 200 + "px";
    }
</script>

</body>
</html>
