<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShakeFit Vending</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: Arial, sans-serif; line-height: 1.6; color: #333; }
        
        /* Header */
        header {
            background: #2ecc71;
            color: white;
            padding: 20px;
            text-align: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        header h1 { font-size: 1.8em; }
        nav { margin-top: 10px; }
        nav a { color: white; text-decoration: none; margin: 0 15px; font-weight: bold; }
        nav a:hover { text-decoration: underline; }

        /* Hero */
        .hero {
            background: #f4f4f4;
            text-align: center;
            padding: 120px 20px 80px;
        }
        .hero h2 { font-size: 2em; color: #2ecc71; }
        .hero p { font-size: 1.2em; margin: 10px 0; }
        .hero button {
            background: #e74c3c;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .hero button:hover { background: #c0392b; }

        /* Sections */
        section { padding: 40px 20px; max-width: 900px; margin: auto; }
        h2 { font-size: 1.8em; color: #2ecc71; text-align: center; margin-bottom: 20px; }
        p { font-size: 1.1em; margin-bottom: 20px; }
        ul { list-style: none; }
        ul li { margin-bottom: 10px; padding-left: 20px; position: relative; }
        ul li:before { content: "✔"; color: #2ecc71; position: absolute; left: 0; }

        /* Backgrounds */
        #about { background: #f9f9f9; }
        #gyms { background: white; }
        #products { background: #f9f9f9; }
        #contact { background: white; }
        #gyms a, #contact a { color: #2ecc71; text-decoration: none; }
        #gyms a:hover, #contact a:hover { text-decoration: underline; }

        /* Products Grid */
        .products-grid {
            display: flex;
            gap: 20px;
            justify-content: center;
            flex-wrap: wrap;
        }
        .product-card {
            background: white;
            border: 1px solid #ddd;
            padding: 15px;
            width: 180px;
            text-align: center;
            border-radius: 5px;
        }
        .product-card img { max-width: 100%; height: auto; }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px;
            font-size: 0.9em;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero { padding: 100px 10px 60px; }
            .hero h2 { font-size: 1.5em; }
            nav a { margin: 0 10px; font-size: 0.9em; }
            .products-grid { flex-direction: column; align-items: center; }
            .product-card { width: 70%; }
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

    <section class="hero" id="home">
        <h2>Fuel Fitness, Boost Profits</h2>
        <p>Protein Shakes for Gyms in Luxembourg</p>
        <button onclick="document.getElementById('gyms').scrollIntoView({behavior: 'smooth'});">Partner With Us</button>
    </section>

    <section id="about">
        <h2>Who We Are</h2>
        <p>ShakeFit Vending brings high-quality protein shakes to gyms across Luxembourg. We make post-workout nutrition fast, affordable, and effortless—boosting gym member satisfaction and creating new revenue for owners. Our vending machines are the perfect addition to any fitness space.</p>
    </section>

    <section id="gyms">
        <h2>Why Partner With ShakeFit?</h2>
        <p>Add value to your gym with no risk or cost.</p>
        <ul>
            <li>No upfront cost – we install and maintain for free.</li>
            <li>Earn passive income – keep 25% of every sale.</li>
            <li>Happy members – convenient shakes they’ll love.</li>
            <li>Risk-free – try it for 30 days, no commitment.</li>
        </ul>
        <p>Ready to start? <a href="#contact">Contact us!</a></p>
    </section>

    <section id="products">
        <h2>Our Protein Shakes</h2>
        <p>Ready-to-drink shakes with 20g protein and low sugar—perfect for post-workout recovery.</p>
        <div class="products-grid">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1622483767028-3b14f6696a74?q=80&w=300" alt="Chocolate">
                <h3>Chocolate</h3>
                <p>Rich and bold</p>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1579721850002-a66ba8b39807?q=80&w=300" alt="Vanilla">
                <h3>Vanilla</h3>
                <p>Smooth and classic</p>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1553787499-6f913386a9a6?q=80&w=300" alt="Strawberry">
                <h3>Strawberry</h3>
                <p>Fruity and fresh</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Get in Touch</h2>
        <p>Gym owners—reach out to bring ShakeFit to your space! Questions? We’re here.</p>
        <p>Email: <a href="mailto:your-email@example.com">your-email@example.com</a></p>
        <p>Phone: +352-123-456</p>
    </section>

    <footer>
        <p>© 2025 ShakeFit Vending. Luxembourg. All rights reserved.</p>
    </footer>
</body>
</html>
