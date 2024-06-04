# Frooha<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Afrah Mohammednur</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #4CAF50;
            color: white;
            text-align: center;
            padding: 1em 0;
        }
        nav {
            display: flex;
            justify-content: center;
            background: #333;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #ddd;
            color: black;
        }
        section {
            padding: 20px;
            margin: 10px;
        }
        #game {
            margin: 20px 0;
        }
    </style>
</head>
<body>

<header>
    <h1>Afrah Mohammednur</h1>
    <p>Pharmacy Student and Life Enthusiast</p>
</header>

<nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
</nav>

<section id="about">
    <h2>About Me</h2>
    <p>I was born and raised in Addis Ababa, Ethiopia. Currently, I am studying pharmacy and I love my life, Alhamdulillah.</p>
</section>

<section id="projects">
    <h2>Projects</h2>
    <p>Here you can showcase your projects or any work you've done. Feel free to add details about your projects here.</p>
</section>

<section id="contact">
    <h2>Contact</h2>
    <p>You can reach me at: <a href="mailto:your-email@example.com">your-email@example.com</a></p>
</section>

<section id="game">
    <h2>Guess the Number Game</h2>
    <p>Try to guess the number between 1 and 100!</p>
    <input type="number" id="guess" placeholder="Enter your guess">
    <button onclick="checkGuess()">Submit</button>
    <p id="result"></p>
</section>

<script>
    let randomNumber = Math.floor(Math.random() * 100) + 1;

    function checkGuess() {
        let userGuess = document.getElementById('guess').value;
        let result = document.getElementById('result');

        if (userGuess == randomNumber) {
            result.textContent = 'Congratulations! You guessed the number.';
        } else if (userGuess > randomNumber) {
            result.textContent = 'Too high! Try again.';
        } else {
            result.textContent = 'Too low! Try again.';
        }
    }
</script>

</body>
</html>
