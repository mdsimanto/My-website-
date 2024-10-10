<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Security Your Email</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        .login-box {
            text-align: center;
        }
        input {
            display: block;
            margin: 10px auto;
            padding: 10px;
            width: 200px;
            border: none;
            border-radius: 5px;
        }
        button {
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="login-box">
        <h1>Login</h1>
        <input type="text" id="username" placeholder="Username">
        <input type="password" id="password" placeholder="Password">
        <button onclick="login()">Login</button>
        <p id="error-message" style="color: red;"></p>
    </div>

    <script>
        function login() {
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;

            // Username and Password Validation
            if (username === "MD SIFAT" && password === "1960171440") {
                window.location.href = "mainpage.html"; // Redirect to main page
            } else {
                document.getElementById("error-message").textContent = "Incorrect Username or Password!";
            }
        }
    </script>
</body>
</html>
