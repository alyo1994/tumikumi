<!DOCTYPE html>
<html>
<head>
  <title>Tumi Website</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <header>
    <h1>Tumi</h1>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Products</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <h2>Welcome to Tumi</h2>
    <p>Tumi is a leading brand in travel and lifestyle products.</p>
  </main>
  <footer>
    <p>Copyright Tumi</p>
  </footer>
  <script src="script.js"></script>
</body>
</html>
body {
  font-family: Arial, sans-serif;
  color: #333;
}

header {
  background-color: #E60073;
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
}

footer {
  background-color: #E60073;
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
