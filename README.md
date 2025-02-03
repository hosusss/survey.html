# survey.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>404 Error</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #ffecf0;
            text-align: center;
            padding: 50px;
        }
        .error {
            font-size: 50px;
            color: #ff6f61;
        }
        .message {
            font-size: 24px;
            margin: 20px 0;
            color: #5d5d5d;
        }
        .question {
            font-size: 28px;
            color: #e91e63;
            font-weight: bold;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            color: #fff;
            background-color: #e91e63;
            border: none;
            cursor: pointer;
            margin-top: 20px;
        }
        button:hover {
            background-color: #c2185b;
        }
    </style>
</head>
<body>
    <div class="error">404 Error - Heart Not Found</div>
    <div class="message">It seems like the page you're looking for is lost... Just like my heart.</div>
    <div class="question" id="valentine-question">Will you be my Valentine?</div>
    <button onclick="checkAnswer(true)">Yes</button>
    <button onclick="checkAnswer(false)">No</button>

    <script>
        function checkAnswer(isYes) {
            const questionElement = document.getElementById("valentine-question");
            if (isYes) {
                questionElement.innerHTML = "Yay! You made my heart skip a beat!";
            } else {
                questionElement.innerHTML = "Are you sure? My heart's still waiting...";
                setTimeout(() => {
                    questionElement.innerHTML = "Will you be my Valentine?";
                }, 2000);
            }
        }
    </script>
</body>
</html>
