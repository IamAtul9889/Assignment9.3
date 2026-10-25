```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Landing Page</title>

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #f8fafc;
        }

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            background: #1e293b;
            color: white;
            flex-wrap: wrap;
            gap: 15px;
        }

        nav {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        nav a {
            color: white;
            text-decoration: none;
        }

        .hero {
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            gap: 30px;
            padding: 50px 8%;
        }

        .hero h1 {
            font-size: clamp(2rem, 4vw, 3rem);
            color: #1e293b;
        }

        .hero p {
            line-height: 1.7;
        }

        .hero img {
            width: 100%;
            max-width: 100%;
            border-radius: 12px;
        }

        .features {
            padding: 30px 8%;
            text-align: center;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(3, minmax(0, 1fr));
            gap: 20px;
        }

        .card {
            display: flex;
            flex-direction: column;
            align-items: center;
            background: white;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 2px 8px #00000015;
        }

        .card p {
            line-height: 1.6;
        }

        .button {
            display: inline-block;
            background: #2563eb;
            color: white;
            padding: 12px 20px;
            text-decoration: none;
            border-radius: 6px;
        }

        footer {
            background: #1e293b;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
        }

        @media (max-width: 700px) {
            header {
                flex-direction: column;
            }

            .hero {
                grid-template-columns: 1fr;
                padding: 30px 5%;
            }

            .cards {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

<header>
    <h2>WebStart</h2>
    <nav>
        <a href="#">Home</a>
        <a href="#features">Features</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero">
    <div>
        <h1>Build Your Future with Technology</h1>
        <p>Learn new skills and create modern, responsive websites using HTML and CSS.</p>
        <a href="#features" class="button">Explore Features</a>
    </div>

    <img src="https://picsum.photos/id/0/600/400" alt="Laptop on a desk">
</section>

<section class="features" id="features">
    <h2>Our Features</h2>

    <div class="cards">
        <div class="card">
            <h3>Easy Learning</h3>
            <p>Learn web development step by step.</p>
        </div>

        <div class="card">
            <h3>Responsive Design</h3>
            <p>Create websites for mobile and desktop.</p>
        </div>

        <div class="card">
            <h3>Modern Layouts</h3>
            <p>Build layouts using Grid and Flexbox.</p>
        </div>
    </div>
</section>

<footer id="contact">
    <p>© 2026 WebStart. All rights reserved.</p>
</footer>

</body>
</html>
```