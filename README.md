<!DOCTYPE html>
<html>
<head>
  <title>Dolphin Website</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <header>
    <h1>Dolphin Website</h1>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <h2>Welcome to the Dolphin Website</h2>
    <p>Dolphins are intelligent and friendly aquatic mammals.</p>
    <img src="dolphin.jpg" alt="A dolphin swimming in the ocean">
  </main>
  <footer>
    <p>Copyright Dolphin Website</p>
  </footer>
  <script src="script.js"></script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  color: #333;
  background-image: url("ocean.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

header {
  background-color: #0077be;
  color: #fff;
  padding: 1em;
}

header h1 {
  margin: 0;
}

header nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

header nav ul li {
  display: inline-block;
  margin-right: 1em;
}

header nav ul li a {
  color: #fff;
  text-decoration: none;
}

main {
  padding: 1em;
  text-align: center;
}

footer {
  background-color: #0077be;
  color: #fff;
  padding: 1em;
  text-align: center;
}
// Add functionality to the navigation menu
const navLinks = document.querySelectorAll("header nav a");
navLinks.forEach(link => {
  link.addEventListener("click", e => {
    e.preventDefault();
    console.log(`Navigating to ${e.target.href}`);
  });
});
