# BBB.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Your Website</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f8f9fa;
      color: #333;
    }

    header {
      background: #1a1a1a;
      padding: 20px;
      color: #fff;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      padding: 15px;
      background: #333;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      text-decoration: underline;
    }

    .hero {
      height: 60vh;
      background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://picsum.photos/1600/900');
      background-size: cover;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      text-align: center;
      padding: 20px;
    }

    .hero h1 {
      font-size: 3rem;
      margin: 0;
    }

    .container {
      max-width: 1000px;
      margin: 40px auto;
      padding: 20px;
    }

    footer {
      background: #1a1a1a;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Your Website Name</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Projects</a>
    <a href="#">Contact</a>
  </nav>

  <section class="hero">
    <h1>Welcome to My Website</h1>
  </section>

  <div class="container">
    <h2>About Me</h2>
    <p>
      This is a clean and simple template you can use for your GitHub Pages site.
      Replace this text with your own content.
    </p>

    <h2>Projects</h2>
    <p>Showcase your work here.</p>

    <h2>Contact</h2>
    <p>Put links or contact info here.</p>
  </div>

  <footer>
    <p>© 2025 Your Name. All rights reserved.</p>
  </footer>
</body>
</html>
