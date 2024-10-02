clothing-store/
├── index.html
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

├── styles.css
/* General Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f9f9f9;
    color: #333;
}

header {
    background-color: #333;
    color: white;
    padding: 20px;
    text-align: center;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header .logo {
    font-size: 24px;
    font-weight: bold;
}

header nav ul {
    list-style: none;
    display: flex;
}

header nav ul li {
    margin-left: 20px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

.banner {
    background-image: url('https://via.placeholder.com/1200x400');
    background-size: cover;
    background-position: center;
    text-align: center;
    padding: 100px 20px;
    color: white;
}

.banner h1 {
    font-size: 48px;
}

.banner p {
    font-size: 18px;
    margin: 20px 0;
}

.shop-now-btn {
    background-color: #ff6347;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    font-size: 18px;
    border-radius: 5px;
}

.product-section {
    padding: 50px 20px;
    text-align: center;
}

.product-section h2 {
    font-size: 32px;
    margin-bottom: 20px;
}

.product-grid {
    display: flex;
    justify-content: center;
    gap: 20px;
}

.product-card {
    background-color: white;
    border: 1px solid #ccc;
    padding: 20px;
    width: 250px;
    text-align: center;
    border-radius: 10px;
}

.product-card img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
}

.product-card h3 {
    font-size: 18px;
    margin: 15px 0;
}

.product-card p {
    font-size: 16px;
    color: #555;
}

.add-to-cart-btn {
    background-color: #007bff;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.add-to-cart-btn:hover {
    background-color: #0056b3;
}

#about, #contact {
    padding: 50px 20px;
    text-align: center;
    background-color: #f0f0f0;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px;
}

└── script.js
// Simple Cart Functionality
const cart = [];

document.querySelectorAll('.add-to-cart-btn').forEach(button => {
    button.addEventListener('click', () => {
        const productName = button.getAttribute('data-product');
        const productPrice = parseFloat(button.getAttribute('data-price'));
        
        cart.push({ name: productName, price: productPrice });
        alert(`${productName} has been added to your cart.`);
        console.log(cart);
    });
});

