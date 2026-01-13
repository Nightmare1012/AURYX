# AURYX
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="AURYX Pakistan: Premium hybrid perfumes for men and women. Discover versatile scents that blend elegance and allure. Shop now!">
    <meta name="keywords" content="hybrid perfumes, unisex fragrances, AURYX Pakistan, men's perfume, women's perfume">
    <title>AURYX Pakistan - Hybrid Perfumes for Men and Women</title>
    <style>
        /* Global Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        h1, h2, h3 {
            font-weight: bold;
        }
        a {
            text-decoration: none;
            color: #FFD700;
        }
        a:hover {
            color: #D32F2F;
        }
        img {
            max-width: 100%;
            height: auto;
        }

        /* Header */
        header {
            background-color: #D32F2F;
            color: #FFD700;
            padding: 20px;
            text-align: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 10px 0 0;
        }
        nav ul li {
            display: inline;
            margin: 0 15px;
        }
        nav ul li a {
            color: #FFD700;
            font-weight: bold;
        }

        /* Sections */
        section {
            padding: 80px 20px 40px;
            max-width: 1200px;
            margin: 0 auto;
        }
        #hero {
            background: linear-gradient(to right, #D32F2F, #FFD700);
            color: white;
            text-align: center;
            padding: 150px 20px 100px;
        }
        #hero h2 {
            font-size: 3em;
            margin-bottom: 20px;
        }
        #hero p {
            font-size: 1.2em;
        }
        .btn {
            background-color: #FFD700;
            color: #D32F2F;
            padding: 15px 30px;
            border: none;
            border-radius: 5px;
            font-size: 1.1em;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .btn:hover {
            background-color: #D32F2F;
            color: #FFD700;
        }

        /* About */
        #about {
            background-color: white;
            text-align: center;
        }

        /* Products */
        #products {
            background-color: #f9f9f9;
        }
        .filter-buttons {
            text-align: center;
            margin-bottom: 20px;
        }
        .filter-buttons button {
            margin: 0 10px;
            padding: 10px 20px;
            background: #D32F2F;
            color: #FFD700;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .filter-buttons button:hover {
            background: #FFD700;
            color: #D32F2F;
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .product {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            overflow: hidden;
            text-align: center;
            transition: transform 0.3s;
            display: block;
        }
        .product.hidden {
            display: none;
        }
        .product:hover {
            transform: translateY(-5px);
        }
        .product img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .product h3 {
            margin: 15px 0;
            color: #D32F2F;
        }
        .product p {
            padding: 0 15px;
        }

        /* Cart */
        #cart {
            position: fixed;
            top: 80px;
            right: 20px;
            background: white;
            border: 1px solid #D32F2F;
            padding: 10px;
            width: 250px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            display: none;
        }
        #cart.show {
            display: block;
        }
        #cart-toggle {
            background: #FFD700;
            color: #D32F2F;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        /* Testimonials */
        #testimonials {
            background-color: white;
        }
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        .testimonial {
            background: #f9f9f9;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }

        /* Blog */
        #blog {
            background-color: #f9f9f9;
        }
        .blog-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }
        .blog-post {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        /* FAQ */
        #faq {
            background-color: white;
        }
        .faq-item {
            margin-bottom: 20px;
        }
        .faq-question {
            background: #D32F2F;
            color: #FFD700;
            padding: 10px;
            cursor: pointer;
            border-radius: 5px;
        }
        .faq-answer {
            display: none;
            padding: 10px;
            background: #f9f9f9;
        }

        /* Newsletter */
        #newsletter {
            background-color: #D32F2F;
            color: #FFD700;
            text-align: center;
            padding: 40px 20px;
        }
        #newsletter form {
            max-width: 400px;
            margin: 0 auto;
        }
        #newsletter input {
            width: 70%;
            padding: 10px;
            border: none;
            border-radius: 5px;
        }
        #newsletter button {
            width: 25%;
            padding: 10px;
        }

        /* Contact */
        #contact {
            background-color: #f9f9f9;
        }
        #contact .contact-info {
            text-align: center;
            margin-bottom: 20px;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
        }
        footer .social-links a {
            margin: 0 10px;
            color: #FFD700;
        }

        /* Responsive */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2em;
            }
            #hero h2 {
                font-size: 2em;
            }
            nav ul li {
                display: block;
                margin: 10px 0;
            }
            #cart {
                width: 200px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>AURYX Pakistan</h1>
        <nav>
            <ul>
                <li><a href="#hero">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#blog">Tips</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
        <button id="cart-toggle">Cart (0)</button>
    </header>

    <div id="cart">
        <h3>Your Cart</h3>
        <ul id="cart-items"></ul>
        <p>Total: $<span id="cart-total">0.00</span></p>
        <button class="btn" onclick="checkout()">Checkout</button>
    </div>

    <section id="hero">
        <h2>Hybrid Perfumes for Men & Women</h2>
        <p>Empower your confidence or radiate elegance. Unisex scents that redefine luxury for him, her, or both.</p>
        <a href="#products" class="btn">Explore Now</a>
    </section>

    <section id="about">
        <h2>About AURYX</h2>
        <p>At AURYX Pakistan, we specialize in hybrid perfumes designed for both men and women. Our unique blends combine masculine strength with feminine grace, creating versatile fragrances that suit any occasion. Crafted with premium ingredients, each scent is a masterpiece of innovation and style.</p>
    </section>

    <section id="products">
        <h2>Our Hybrid Perfumes</h2>
        <div class="filter-buttons">
            <button onclick="filterProducts('all')">All</button>
            <button onclick="filterProducts('fresh')">Fresh</button>
            <button onclick="filterProducts('bold')">Bold</button>
            <button onclick="filterProducts('timeless')">Timeless</button>
        </div>
        <div class="product-grid">
            <div class="product" data-category="fresh">
                <img src="https://via.placeholder.com/250x200/FFD700/D32F2F?text=Hybrid+Bliss" alt="Hybrid Bliss Perfume - Fresh scent for everyday confidence">
                <h3>Hybrid Bliss</h3>
                <p>A fresh, woody scent with floral notes – perfect for everyday wear. Empower your confidence.</p>
                <button class="btn add-to-cart" data-name="Hybrid Bliss" data-price="49.99">Add to Cart - $49.99</button>
            </div>
            <div class="product" data-category="bold">
                <img src="https://via.placeholder.com/250x200/D32F2F/FFD700?text=Mystic+Blend" alt="Mystic Blend Perfume - Bold scent for mysterious allure">
                <h3>Mystic Blend</h3>
                <p>Spicy and sweet undertones for a bold, mysterious vibe. Radiate elegance on date nights.</p>
                <button class="btn add-to-cart" data-name="Mystic Blend" data-price="59.99">Add to Cart - $59.99</button>
            </div>
            <div class="product" data-category="timeless">
                <img src="https://via.placeholder.com/250x200/FFD700/D32F2F?text=Eternal+Echo" alt="Eternal Echo Perfume - Timeless scent for sophistication">
                <h3>Eternal Echo</h3>
                <p>Citrus and musk fusion for timeless appeal. Versatile for office or evenings.</p>
                <button class="btn add-to-cart" data-name="Eternal Echo" data-price="54.99">Add to Cart - $54.99</button>
            </div>
            <div class="product" data-category="bold">
                <img src="https://via.placeholder.com/250x200/D32F2F/FFD700?text=Velvet+Harmony" alt="Velvet Harmony Perfume - Bold scent for harmony">
                <h3>Velvet Harmony</h3>
                <p>Smooth vanilla and leather notes for sophistication. Blend strength and grace.</p>
                <button class="btn add-to-cart" data-name="Velvet Harmony" data-price="64.99">Add to Cart - $64.99</button>
            </div>
        </div>
    </section>

    <section id="testimonials">
        <h2>What Our Customers Say</h2>
        <div class="testimonial-grid">
            <div class="testimonial">
                <p>"As a man, I love how these hybrid scents boost my confidence without being overpowering." - Ahmed, Karachi</p>
            </div>
            <div class="testimonial">
                <p>"Perfect for women like me who want elegance and versatility. My go-to for dates!" - Sara, Lahore</p>
            </div>
        </div>
    </section>

    <section id="blog">
        <h2>Perfume Tips & Inspiration</h2>
        <div class="blog-grid">
            <div class="blog-post">
                <h3>For Him: Office Scents That Impress</h3>
                <p>Choose fresh, woody notes like Hybrid Bliss to project professionalism and confidence at work.</p>
            </div>
            <div class="blog-post">
                <h3>For Her: Date Night Fragrances</h3>
                <p>Opt for bold, mysterious blends like Mystic Blend to add allure and elegance to your evening.</p>
            </div>
        </div>
    </section>

    <section id="faq">
        <h2>Frequently Asked Questions</h2>
        <div class="faq-item">
            <div class="faq-question" onclick="toggleFAQ(this)">What makes hybrid perfumes unique?</div>
            <div class="faq-answer">They blend masculine and feminine notes for versatility, appealing to both genders.</div>
        </div>
        <div class="faq-item">
            <div class="faq-question" onclick="toggleFAQ(this)">Are they suitable for men and women?</div>
            <div class="faq-answer">Yes! Designed for unisex appeal, perfect for anyone seeking elegance or confidence.</div>
        </div>
    </section>

    <section id="newsletter">
        <h2>Stay Updated</h2>
        <p>Subscribe for exclusive deals and new scent launches.</p>
        <form id="newsletter-form">
            <input type="email" placeholder="Your Email" required>
            <button type="submit" class="btn">Subscribe</button>
        </form>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <div class="contact-info">
            <p>Email: info@aurypakistan.com | Phone: +92-123-456789</p>
            <img src="https://via.placeholder.com/400x200/D32F2F/FFD700?text=Map+Location" alt="Map of AURYX Pakistan location">
        </div>
        <form>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" rows="5" required></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2023 AURYX Pakistan. All rights reserved.</p>
        <div class="social-links">
            <a href="#">Instagram</a> | <a href="#">Facebook</a> | <a href="#">Twitter</a>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Cart functionality
        let cart = [];
        let total = 0;
        document.querySelectorAll('.add-to-cart').forEach(btn => {
            btn.addEventListener('click', () => {
                const name = btn.dataset.name;
                const price = parseFloat(btn.dataset.price);
                cart.push({ name, price });
                total += price;
                updateCart();
            });
        });
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            cartItems.innerHTML = cart.map(item => `<li>${item.name} - $${item.price}</li>`).join('');
