<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* Inline CSS for Comic Sans MS */
    body {
      font-family: "Comic Sans MS", cursive, sans-serif;
      margin: 0;
      padding: 0;
    }

    /* Navbar Styling */
    .navbar {
      background-color: #6A0DAD;
      padding: 10px;
      text-align: center;
    }

    .navbar ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    .navbar ul li {
      display: inline;
      margin: 0 15px;
    }

    .navbar ul li a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s ease-in-out;
    }

    .navbar ul li a:hover {
      color: #FFD700;
    }

    /* Hero Section Styling */
    .hero {
      position: relative;
      height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
      overflow: hidden;
    }

    /* YouTube Video Background */
    .hero iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
      opacity: 0.7;
    }

    .hero h1 {
      font-size: 3.5rem;
      margin: 0;
      text-shadow: 2px 2px 5px #000;
      animation: slideIn 2s ease-out forwards;
    }

    .hero h2 {
      font-size: 2rem;
      margin: 10px 0;
      color: #FFD700;
      animation: zoomIn 3s ease-out forwards;
    }

    .hero p {
      font-size: 1.2rem;
      margin-top: 15px;
    }

    /* Button Style */
    .hero button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #FFD700;
      color: #6A0DAD;
      border: none;
      font-size: 1.2rem;
      font-weight: bold;
      cursor: pointer;
      border-radius: 5px;
      transition: transform 0.3s ease-in-out;
    }

    .hero button:hover {
      transform: scale(1.1);
    }

    /* Animations */
    @keyframes slideIn {
      from {
        transform: translateY(-50px);
      }
      to {
        transform: translateY(0);
      }
    }

    @keyframes zoomIn {
      from {
        transform: scale(0.8);
        opacity: 0.5;
      }
      to {
        transform: scale(1);
        opacity: 1;
      }
    }
  </style>
</head>
<body>
  <!-- Navigation Bar -->
  <nav class="navbar">
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="portfolio.html">Portfolio</a></li>
      <li><a href="contact.html">Contact</a></li>
      <li><a href="game.html">Game</a></li>
    </ul>
  </nav>

  <!-- Hero Section with YouTube Video Background -->
  <section class="hero">
    <!-- Embedded YouTube Video -->
    <iframe src="https://www.youtube.com/embed/ET-XLp5tUz8?autoplay=1&mute=1&loop=1&playlist=ET-XLp5tUz8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

    <h1>Welcome to My Website</h1>
    <h2>San Francisco Bay University</h2>
    <p>Explore my portfolio, learn about me, and check out my projects!</p>
    <button onclick="window.location.href='https://www.sfbu.edu/'">Learn More</button>
  </section>

  <script>
    // JavaScript for Button Interaction
    function showWelcomeMessage() {
      alert("Welcome to San Francisco Bay University! Explore our website.");
    }
  </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Me</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* General Styling */
    body {
      font-family: "Comic Sans MS", cursive, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f9;
      color: #333;
    }

    /* Navbar Styling */
    .navbar {
      background-color: #6A0DAD;
      padding: 10px;
      text-align: center;
    }

    .navbar ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    .navbar ul li {
      display: inline;
      margin: 0 15px;
    }

    .navbar ul li a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s ease-in-out;
    }

    .navbar ul li a:hover {
      color: #FFD700;
    }

    /* Hero Section */
    .hero-about {
      position: relative;
      text-align: center;
      padding: 50px 20px;
      background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://www.sfbu.edu/sites/default/files/styles/full_node_banner/public/2021-11/Campus.jpeg') no-repeat center center/cover;
      color: white;
    }

    .hero-about h1 {
      font-size: 3rem;
      margin: 0;
      animation: fadeInDown 2s ease;
    }

    .hero-about p {
      font-size: 1.2rem;
      margin-top: 20px;
      animation: fadeInUp 2s ease;
    }

    /* About Section */
    .about-container {
      padding: 40px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .about-container h2 {
      text-align: center;
      font-size: 2.5rem;
      color: #6A0DAD;
      margin-bottom: 20px;
      animation: fadeIn 2s ease;
    }

    .about-container .about-content {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .about-box {
      flex: 1 1 calc(33.333% - 20px);
      background-color: white;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
      animation: fadeIn 2s ease;
    }

    .about-box:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.4);
    }

    .about-box h3 {
      color: #6A0DAD;
      margin-top: 0;
    }

    .about-box p {
      line-height: 1.6;
    }

    /* Animations */
    @keyframes fadeInDown {
      from {
        opacity: 0;
        transform: translateY(-20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    /* Mobile Responsiveness */
    @media (max-width: 768px) {
      .about-box {
        flex: 1 1 calc(100% - 20px);
      }

      .hero-about h1 {
        font-size: 2.5rem;
      }

      .hero-about p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <!-- Navigation Bar -->
  <nav class="navbar">
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="portfolio.html">Portfolio</a></li>
      <li><a href="contact.html">Contact</a></li>
      <li><a href="game.html">Game</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero-about">
    <h1>About Me</h1>
    <p>Learn more about my journey and San Francisco Bay University.</p>
  </section>

  <!-- About Section -->
  <section class="about-container">
    <h2>Who I Am</h2>
    <div class="about-content">
      <div class="about-box">
        <h3>Education</h3>
        <p>My name is <strong>Sanjida Ahamed</strong>, and I am currently studying at San Francisco Bay University, a renowned institution located in the heart of Silicon Valley. It offers top-tier programs in computer science and business management.</p>
      </div>
      <div class="about-box">
        <h3>Skills</h3>
        <p>I specialize in web development, JavaScript, and modern frameworks. I am also learning advanced design concepts and enjoy working on interactive web applications.</p>
      </div>
      <div class="about-box">
        <h3>Interests</h3>
        <p>In addition to coding, I am passionate about hiking, exploring nature, and engaging in cultural events. I love blending creativity and technology to build impactful projects.</p>
      </div>
    </div>
  </section>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* General Styling */
    body {
      font-family: "Comic Sans MS", cursive, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f9;
      color: #333;
    }

    /* Navbar Styling */
    .navbar {
      background: linear-gradient(to right, #0066cc, #003366);
      padding: 15px;
      text-align: center;
    }

    .navbar ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    .navbar ul li {
      display: inline;
      margin: 0 15px;
    }

    .navbar ul li a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s ease-in-out;
    }

    .navbar ul li a:hover {
      color: #66cc33;
    }

    /* Portfolio Section */
    .portfolio-container {
      padding: 60px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .portfolio-container h2 {
      text-align: center;
      font-size: 2.8rem;
      color: #6A0DAD;
      margin-bottom: 30px;
    }

    .portfolio-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .portfolio-item {
      background: white;
      border-radius: 10px;
      padding: 20px;
      width: calc(33% - 40px);
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      text-align: center;
    }

    .portfolio-item:hover {
      transform: scale(1.05);
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.4);
    }

    .portfolio-item h3 {
      color: #6A0DAD;
    }

    .portfolio-item p {
      line-height: 1.6;
    }

    .portfolio-item a {
      background-color: #66cc33;
      color: white;
      padding: 10px 20px;
      border-radius: 5px;
      text-decoration: none;
      transition: background-color 0.3s ease;
    }

    .portfolio-item a:hover {
      background-color: #003366;
    }

    /* Mobile Responsiveness */
    @media (max-width: 768px) {
      .portfolio-item {
        width: calc(100% - 40px);
      }
    }

  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar">
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="portfolio.html">Portfolio</a></li>
      <li><a href="contact.html">Contact</a></li>
      <li><a href="game.html">Game</a></li>
    </ul>
  </nav>

  <!-- Portfolio Section -->
  <section class="portfolio-container">
    <h2>My Projects</h2>
    <div class="portfolio-grid">
      <!-- Project 1 -->
      <div class="portfolio-item">
        <h3>Car Dealership System</h3>
        <p>A database system project built in SQL for managing car dealership operations and data.</p>
        <a href="https://drive.google.com/file/d/1EPrMxy9T5f9GAEw_k24j0Cm3hUHg3nwR/view?usp=drive_link" target="_blank">View Project</a>
      </div>

      <!-- Project 2 -->
      <div class="portfolio-item">
        <h3>Python Pizza Inventory</h3>
        <p>A Python-based food inventory management system for a pizza store, including inventory tracking and menu management.</p>
        <a href="https://drive.google.com/file/d/1hRKm0XlYjPLHqazCoEw_dXtQfWUsk4dM/view?usp=drive_link" target="_blank">View Project</a>
      </div>

      <!-- Project 3 -->
      <div class="portfolio-item">
        <h3>Linux Food Menu System</h3>
        <p>A Linux-based system for managing food menus and recipes, developed with shell scripting and custom tools.</p>
        <a href="https://drive.google.com/file/d/1YIapaJ9cIZDFktZ7U80VG40EJh2om7lW/view?usp=drive_link" target="_blank">View Project</a>
      </div>
    </div>
  </section>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact Me</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    body {
      font-family: "Comic Sans MS", cursive, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #1a1a1a;
      color: white;
    }

    .navbar {
      background: linear-gradient(to right, #0066cc, #003366);
      padding: 15px;
      text-align: center;
    }

    .navbar ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    .navbar ul li {
      display: inline;
      margin: 0 15px;
    }

    .navbar ul li a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s ease-in-out;
    }

    .navbar ul li a:hover {
      color: #66cc33;
    }

    /* Contact Form Section */
    .contact-container {
      padding: 60px 20px;
      max-width: 800px;
      margin: auto;
      background-color: #003366;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      text-align: center;
    }

    .contact-container h2 {
      font-size: 2.8rem;
      color: #66cc33;
      margin-bottom: 30px;
    }

    .contact-container form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .contact-container input,
    .contact-container textarea {
      padding: 10px;
      font-size: 1rem;
      border: 1px solid #ddd;
      border-radius: 5px;
    }

    .contact-container button {
      padding: 10px;
      font-size: 1.2rem;
      background-color: #66cc33;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .contact-container button:hover {
      background-color: #003366;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar">
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="portfolio.html">Portfolio</a></li>
      <li><a href="contact.html">Contact</a></li>
      <li><a href="game.html">Game</a></li>
    </ul>
  </nav>

  <!-- Contact Section -->
  <section class="contact-container">
    <h2>Contact Me</h2>
    <form action="https://formspree.io/f/mzzbqbrr" method="POST">
      <input type="text" name="name" placeholder="Your Name" required>
      <input type="email" name="email" placeholder="Your Email" required>
      <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Guess the Number Game</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* General Styling */
    body {
      font-family: "Comic Sans MS", cursive, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #00c6ff, #0072ff);
      color: white;
    }

    /* Navbar Styling */
    .navbar {
      background: linear-gradient(to right, #0066cc, #003366);
      padding: 15px;
      text-align: center;
    }

    .navbar ul {
      margin: 0;
      padding: 0;
      list-style: none;
    }

    .navbar ul li {
      display: inline;
      margin: 0 15px;
    }

    .navbar ul li a {
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: color 0.3s ease-in-out;
    }

    .navbar ul li a:hover {
      color: #66cc33;
    }

    /* Game Container */
    .game-container {
      background-color: #003366;
      max-width: 600px;
      margin: 50px auto;
      padding: 30px;
      border-radius: 10px;
      text-align: center;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
    }

    .game-container h1 {
      font-size: 2.5rem;
      color: #66cc33;
    }

    .game-container p {
      font-size: 1.2rem;
      color: #ffffff;
    }

    .game-container input {
      padding: 10px;
      font-size: 1.2rem;
      border: 1px solid #ddd;
      border-radius: 5px;
      width: 50%;
      margin-bottom: 20px;
    }

    .game-container button {
      padding: 10px 20px;
      font-size: 1.2rem;
      background-color: #66cc33;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .game-container button:hover {
      background-color: #003366;
    }

    .message {
      margin-top: 20px;
      font-size: 1.5rem;
      font-weight: bold;
      color: #ff0099;
    }

    .score {
      margin-top: 20px;
      font-size: 1.2rem;
      color: #ffffff;
    }

    .reset-button {
      padding: 10px 20px;
      background-color: #ff0099;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 30px;
      font-size: 1.2rem;
      transition: background-color 0.3s ease;
    }

    .reset-button:hover {
      background-color: #003366;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar">
    <ul>
      <li><a href="home.html">Home</a></li>
      <li><a href="about.html">About</a></li>
      <li><a href="portfolio.html">Portfolio</a></li>
      <li><a href="contact.html">Contact</a></li>
      <li><a href="game.html">Game</a></li>
    </ul>
  </nav>

  <!-- Game Container -->
  <div class="game-container">
    <h1>Guess the Number Game</h1>
    <p>I'm thinking of a number between 1 and 100. Can you guess it?</p>

    <input type="number" id="userGuess" placeholder="Enter your guess" min="1" max="100">
    <button onclick="checkGuess()">Submit Guess</button>

    <p id="hintMessage" class="message"></p>
    <p id="score" class="score">Attempts: 0</p>
    <button id="resetBtn" class="reset-button" onclick="resetGame()" style="display:none;">Play Again</button>
  </div>

  <script>
    // Initialize game variables
    let randomNumber = Math.floor(Math.random() * 100) + 1;  // Random number between 1 and 100
    let attempts = 0;

    // Check user guess
    function checkGuess() {
      const userGuess = parseInt(document.getElementById("userGuess").value);
      const hintMessage = document.getElementById("hintMessage");
      const score = document.getElementById("score");

      // Input validation
      if (isNaN(userGuess) || userGuess < 1 || userGuess > 100) {
        hintMessage.textContent = "Please enter a number between 1 and 100.";
        hintMessage.style.color = "red";
        return;
      }

      attempts++;
      score.textContent = `Attempts: ${attempts}`;

      if (userGuess < randomNumber) {
        hintMessage.textContent = "Too low! Try again.";
        hintMessage.style.color = "orange";
      } else if (userGuess > randomNumber) {
        hintMessage.textContent = "Too high! Try again.";
        hintMessage.style.color = "orange";
      } else {
        hintMessage.textContent = `Congratulations! You guessed the number in ${attempts} attempts.`;
        hintMessage.style.color = "green";
        document.querySelector("button").disabled = true; // Disable the button after correct guess
        document.getElementById("resetBtn").style.display = "block"; // Show the reset button
      }
    }

    // Reset the game
    function resetGame() {
      randomNumber = Math.floor(Math.random() * 100) + 1;  // Generate a new random number
      attempts = 0;
      document.getElementById("userGuess").value = '';  // Clear the input field
      document.getElementById("hintMessage").textContent = '';
      document.getElementById("score").textContent = 'Attempts: 0';
      document.querySelector("button").disabled = false;  // Enable the button again
      document.getElementById("resetBtn").style.display = "none";  // Hide the reset button
    }
  </script>

</body>
</html>

