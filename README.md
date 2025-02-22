<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShakeFit Vending - Protein Shakes for Gyms</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Arial', sans-serif; line-height: 1.6; color: #333; }
        
        /* Header */
        header {
            background: linear-gradient(135deg, #2ecc71, #27ae60);
            color: white;
            padding: 20px;
            text-align: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        header h1 { font-size: 2em; }
        nav { margin-top: 10px; }
        nav a { color: white; text-decoration: none; margin: 0 20px; font-weight: bold; }
        nav a:hover { text-decoration: underline; }

        /* Hero Section */
        .hero {
            background: url('https://images.unsplash.com/photo-1600585154340-be6161a56a0c?q=80&w=2070') no-repeat center/cover;
            color: white;
            text-align: center;
            padding: 150px 20px 100px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.7);
        }
        .hero h2 { font-size: 2.5em; margin-bottom: 10px; }
        .hero p { font-size: 1.2em; margin-bottom: 20px; }
        .hero button {
            background: #e74c3c;
            color: white;
            padding: 12px 25px;
            border: none;
            border-radius: 5px;
            font-size: 1.1em;
            cursor: pointer;
            transition: background 0.3s;
        }
        .hero button:hover { background: #c0392b; }

        /* Sections */
        section { padding: 60px 20px; max-width: 1000px; margin: auto; }
        h2 { font-size: 2em; color: #2ecc71; margin-bottom: 20px; text-align: center; }
        p, ul { font-size: 1.1em; margin-bottom: 20px; }
        ul { list-style: none; padding-left: 0; }
        ul li { margin-bottom: 10px; position: relative; padding-left: 25px; }
        ul li:before { content: "✔"; color: #2ecc71; position: absolute; left: 0; }

        /* About Section */
        #about { background: #f9f9f9; }

        /* Gyms Section */
        #gyms { background: white; }
        #gyms a { color: #2ecc71; text-decoration: none; font-weight: bold; }
        #gyms a:hover { text-decoration: underline; }

        /* Products Section */
        .products-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        .product-card {
            background: #fff;
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 20px;
            width: 200px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .product-card img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }

        /* Contact Section */
        #contact { background: #f9f9f9; }
        #contact form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 500px;
            margin: 0 auto;
        }
        #contact input, #contact textarea {
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1em;
        }
        #contact button {
            background: #2ecc71;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        #contact button:hover { background: #27ae60; }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero { padding: 100px 20px 80px; }
            .hero h2 { font-size: 1.8em; }
            nav a { margin: 0 10px; font-size: 0.9em; }
            .products-grid { flex-direction: column; align-items: center; }
            .product-card { width: 80%; }
        }
    </style>
</head>
<body>
    <header>
        <h1>ShakeFit Vending</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#gyms">For Gyms</a>
            <a href="#products">Products</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <div class="hero" id="home">
        <h2>Fuel Fitness, Boost Profits</h2>
        <p>Protein Shakes for Gyms in Luxembourg</p>
        <button onclick="document.getElementById('gyms').scrollIntoView({behavior: 'smooth'});">Partner With Us</button>
    </div>

    <section id="about">
        <h2>Who We Are</h2>
        <p>ShakeFit Vending delivers high-quality protein shakes to gyms across Luxembourg. We’re here to make post-workout nutrition fast, affordable, and effortless—enhancing the gym experience for members while creating a new revenue stream for owners. With state-of-the-art vending machines, we’re fueling fitness, one shake at a time.</p>
    </section>

    <section id="gyms">
        <h2>Why Partner With ShakeFit?</h2>
        <ul>
            <li>No upfront cost – we install and maintain the machine free of charge.</li>
            <li>Earn passive income – keep 25% of every sale with zero effort.</li>
            <li>Delight your members – offer convenient, healthy shakes they’ll love.</li>
            <li>Risk-free trial – test it for 30 days; if it doesn’t work, we’ll remove it.</li>
        </ul>
        <p>Ready to bring ShakeFit to your gym? <a href="#contact">Contact us today!</a></p>
    </section>

    <section id="products">
        <h2>Our Protein Shakes</h2>
        <p>Premium, ready-to-drink shakes packed with 20g of protein and low sugar. Perfect for post-workout recovery.</p>
        <div class="products-grid">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1622483767028-3b14f6696a74?q=80&w=300" alt="Chocolate Shake">
                <h3>Chocolate</h3>
                <p>Rich and satisfying.</p>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1579721850002-a66ba8b39807?q=80&w=300" alt="Vanilla Shake">
                <h3>Vanilla</h3>
                <p>Smooth and classic.</p>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1553787499-6f913386a9a6?q=80&w=300" alt="Strawberry Shake">
                <h3>Strawberry</h3>
                <p>Fruity and refreshing.</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Get in Touch</h2>
        <p>Gym owners and fitness enthusiasts—reach out to learn more!</p>
        <form action="#" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
            <button type="submit">Send Message</button>
        </form>
        <p>Or email us: <a href="mailto:info@shakefitvending.com">info@shakefitvending.com</a> | Phone: +352-123-456</p>
    </section>

    <footer>
        <p>&copy; 2025 ShakeFit Vending. Luxembourg. All rights reserved.</p>
    </footer>
</body>
</html>
