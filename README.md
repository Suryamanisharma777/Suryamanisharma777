
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Promotional Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>

    <!-- Navbar -->
    <nav>
        <div class="logo">PromoHub</div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#products">Products</a></li>
            <li><a href="#testimonials">Testimonials</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Welcome to PromoHub</h1>
        <p>Your destination for the best products and services</p>
        <a href="#products" class="cta-button">Explore Products</a>
    </section>

    <!-- About Us Section -->
    <section id="about" class="section">
        <h2>About Us</h2>
        <p>At PromoHub, we specialize in promoting quality products and services that add value to your life. Our team is dedicated to helping you find what you need and love.</p>
    </section>

    <!-- Products and Services Section -->
    <section id="products" class="section">
        <h2>Our Products & Services</h2>
        <div class="product-grid">
            <div class="product-card">
                <h3>Product 1</h3>
                <p>Amazing product with top-notch features.</p>
            </div>
            <div class="product-card">
                <h3>Product 2</h3>
                <p>High-quality product for everyday needs.</p>
            </div>
            <div class="product-card">
                <h3>Service 1</h3>
                <p>Professional service that exceeds expectations.</p>
            </div>
            <div class="product-card">
                <h3>Service 2</h3>
                <p>Dedicated service with excellent results.</p>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="section">
        <h2>What Our Clients Say</h2>
        <div class="testimonials">
            <blockquote>
                "PromoHub helped me find the best product, and I couldn't be happier with my choice!"
                <cite>- Alex R.</cite>
            </blockquote>
            <blockquote>
                "The service was excellent and very professional. Highly recommended!"
                <cite>- Jordan K.</cite>
            </blockquote>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <h2>Contact Us</h2>
        <form>
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2023 PromoHub. All rights reserved.</p>
    </footer>

</body>
</html
