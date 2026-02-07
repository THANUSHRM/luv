  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Will You Be My Valentine? ❤️</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            background: linear-gradient(135deg, #ff4d6d, #ff9a9e);
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: 'Segoe UI', sans-serif;
        }

        .box {
            background: white;
            padding: 40px;
            border-radius: 25px;
            text-align: center;
            box-shadow: 0 15px 40px rgba(0,0,0,0.2);
            max-width: 350px;
        }

        h1 {
            color: #ff4d6d;
            margin-bottom: 10px;
        }

        p {
            font-size: 18px;
            color: #333;
        }

        .buttons {
            margin-top: 25px;
        }

        button {
            padding: 12px 25px;
            font-size: 18px;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            margin: 10px;
            transition: 0.3s;
        }

        #yes {
            background: #ff4d6d;
            color: white;
        }

        #no {
            background: #ccc;
        }

        #no:hover {
            position: absolute;
            left: Math.random() * 80 + "%";
            top: Math.random() * 80 + "%";
        }

        .heart {
            font-size: 50px;
            margin-top: 20px;
            display: none;
            animation: beat 1s infinite;
        }

        @keyframes beat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.3); }
        }
    </style>
</head>
<body>

<div class="box">
    <h1>Hello Suchitra</h1>
    <p>Will you be my Valentine?</p>

    <div class="buttons">
        <button id="yes" onclick="sayYes()">NO</button>
        <button id="no" onmouseover="moveNo()">YES</button>
    </div>

    <div class="heart" id="heart">Thank God!</div>
</div>

<script>
    function sayYes() {
        document.getElementById("heart").style.display = "block";
        alert("Yayyy! I’m the luckiest person alive 😍❤️");
    }

    function moveNo() {
        const btn = document.getElementById("no");
        btn.style.position = "absolute";
        btn.style.left = Math.random() * 80 + "%";
        btn.style.top = Math.random() * 80 + "%";
    }
</script>

</body>
</html>
