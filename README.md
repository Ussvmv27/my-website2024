<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clothing Store</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="logo">Fashion Hub</div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="banner">
        <h1>Welcome to Fashion Hub</h1>
        <p>Trendy Clothes at Affordable Prices</p>
        <a href="#products" class="shop-now-btn">Shop Now</a>
    </section>

    <section id="products" class="product-section">
        <h2>Our Collection</h2>
        <div class="product-grid">
            <!-- Product 1 -->
            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="T-shirt">
                <h3>Classic T-Shirt</h3>
                <p>$25.00</p>
                <button class="add-to-cart-btn" data-product="Classic T-Shirt" data-price="25">Add to Cart</button>
            </div>
            <!-- Product 2 -->
            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Jeans">
                <h3>Blue Denim Jeans</h3>
                <p>$40.00</p>
                <button class="add-to-cart-btn" data-product="Blue Denim Jeans" data-price="40">Add to Cart</button>
            </div>
            <!-- Product 3 -->
            <div class="product-card">
                <img src="https://via.placeholder.com/250" alt="Jacket">
                <h3>Leather Jacket</h3>
                <p>$120.00</p>
                <button class="add-to-cart-btn" data-product="Leather Jacket" data-price="120">Add to Cart</button>
            </div>
        </div>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>At Fashion Hub, we provide high-quality, trendy clothing at affordable prices. Whether you're looking for casual wear or something more formal, we have something for everyone.</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>Email: support@fashionhub.com</p>
        <p>Phone: +123 456 7890</p>
    </section>

    <footer>
        <p>&copy; 2024 Fashion Hub. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
