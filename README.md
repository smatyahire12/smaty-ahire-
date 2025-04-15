<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ONE SIDE SHOPPING</title>
    <style>
        /* Animated Background */
        @keyframes colorChange {
            0% { background-color: #ff7f7f; }
            25% { background-color: #7f7fff; }
            50% { background-color: #7fff7f; }
            75% { background-color: #fff77f; }
            100% { background-color: #ff7f7f; }
        }

        /* Slide-in Animation for Header Text */
        @keyframes slideIn {
            0% {
                transform: translateY(-100px);
                opacity: 0;
            }
            100% {
                transform: translateY(0);
                opacity: 1;
            }
        }

        /* Button Hover Animation */
        @keyframes buttonHover {
            0% {
                transform: scale(1);
                background-color: #ff7f7f;
            }
            100% {
                transform: scale(1.1);
                background-color: #ff4040;
            }
        }

        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            animation: colorChange 10s infinite;
            height: 100%;
            background-size: cover;
            background-position: center;
            color: #fff;
        }

        header, section {
            text-align: center;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            animation: slideIn 1s ease-out;
        }

        h1, h2 {
            margin: 0.5em 0;
        }

        .banner {
            background: url('https://via.placeholder.com/1200x300') no-repeat center center/cover;
            height: 300px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2.5em;
            color: white;
            font-weight: bold;
        }

        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            padding: 20px;
            opacity: 0;
            animation: fadeIn 2s ease-out forwards;
        }

        /* Fade-in Animation for Product Container */
        @keyframes fadeIn {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }

        .product {
            background-color: rgba(0, 0, 0, 0.7);
            padding: 20px;
            margin: 20px;
            border-radius: 8px;
            text-align: center;
            width: 250px;
            transition: transform 0.3s ease;
        }

        .product img {
            max-width: 100%;
            border-radius: 8px;
            transition: transform 0.3s ease;
        }

        .product:hover {
            transform: scale(1.1);
        }

        .product:hover img {
            transform: scale(1.2);
        }

        .product-details {
            margin-top: 10px;
        }

        /* Additional Button Hover Animation */
        .product button:hover {
            animation: buttonHover 0.3s forwards;
        }

        .contact-form, .feedback-form {
            width: 100%;
            text-align: center;
            margin-top: 30px;
            padding: 30px;
        }

        .contact-form input, .contact-form textarea,
        .feedback-form input, .feedback-form textarea {
            padding: 15px;
            margin: 10px;
            border-radius: 8px;
            border: 1px solid #ccc;
            width: 85%;
            font-size: 1.1em;
        }

        .contact-form button, .feedback-form button {
            padding: 15px 30px;
            background-color: #ff7f7f;
            color: white;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            font-size: 1.1em;
        }

        .contact-form button:hover, .feedback-form button:hover {
            background-color: #ff4040;
        }

        .info, .about, .product-info {
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.6);
            margin: 10px auto;
            max-width: 1000px;
            border-radius: 10px;
        }

        .form-select {
            margin-bottom: 20px;
            padding: 10px;
            font-size: 1.1em;
            border-radius: 4px;
            border: 1px solid #ccc;
            width: 90%;
        }
    </style>
</head>
<body>

<header>
    <h1>ONE SIDE SHOPPING</h1>
    <p>Find the best products at the best prices!</p>
</header>

<div class="banner">
    Welcome to ONE SIDE SHOPPING!
</div>

<section class="about">
    <h2>About Us</h2>
    <p>ONE SIDE  SHOPPING is your one-stop destination for trendy and affordable fashion. 
    Our mission is to bring you the best products with unbeatable prices and top-notch customer service.</p>
</section>

<section class="info">
    <h2>Information</h2>
    <p>We offer fast delivery, easy returns, and secure payment methods. Our dedicated team ensures every product is quality checked before dispatch.</p>
</section>

<section class="product-info">
    <h2>Product Details</h2>
    <ul>
        <li><strong>Zara:</strong> Stylish and premium quality clothing for all occasions.</li>
        <li><strong>Zudio:</strong> Affordable and everyday fashion essentials.</li>
        <li><strong>Trendz:</strong> Fresh fashion trends at your fingertips.</li>
        <li><strong>H&M:</strong> Fashion-forward pieces for all seasons.</li>
        <li><strong>Mango:</strong> European-style fashion at great prices.</li>
        <li><strong>Uniqlo:</strong> Quality clothing for everyone, every day.</li>
    </ul>
</section>

<!-- Products -->
<div class="container">
    <div class="product">
        <img src="C:\Users\admin\Downloads\ss3.jpeg" alt="Zara">
        <div class="product-details">
            <h3>Zara</h3>
            <p>50.00rs</p>
            <button>Add to Cart</button>
        </div>
    </div>

    <div class="product">
        <img src="C:\Users\admin\Downloads\ss3.jpeg" alt="Zudio">
        <div class="product-details">
            <h3>Zudio</h3>
            <p>30.00rs</p>
            <button>Add to Cart</button>
        </div>
    </div>

    <div class="product">
        <img src="C:\Users\admin\Downloads\ss3.jpeg" alt="Trendz">
        <div class="product-details">
            <h3>Trendz</h3>
            <p>40.00rs</p>
            <button>Add to Cart</button>
        </div>
    </div>

    <!-- New Products -->
    <div class="product">
        <img src="C:\Users\admin\Downloads\ss3.jpeg" alt="H&M">
        <div class="product-details">
            <h3>H&M</h3>
            <p>45.00rs</p>
            <button>Add to Cart</button>
        </div>
    </div>

    <div class="product">
        <img src="C:\Users\admin\Downloads\ss3.jpeg" alt="Mango">
        <div class="product-details">
            <h3>Mango</h3>
            <p>60.00rs</p>
            <button>Add to Cart</button>
        </div>
    </div>

    <div class="product">
        <img src="C:\Users\admin\Downloads\ss3.jpeg" alt="Uniqlo">
        <div class="product-details">
            <h3>Uniqlo</h3>
            <p>55.00rs</p>
            <button>Add to Cart</button>
        </div>
    </div>
</div>

<!-- Contact & Feedback Form -->
<div class="contact-feedback-form">
    <h2>about responce</h2>
    <form>
        <select class="form-select" id="formType" name="formType" onchange="toggleForms()">
            <option value="contact">Contact Us</option>
            <option value="feedback">Feedback</option>
        </select>

        <!-- Contact Us Form -->
        <div id="contactForm" class="contact-form">
            <h3>Contact Us</h3>
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" required></textarea>
            <button type="submit">Submit</button>
        </div>

        <!-- Feedback Form -->
        <div id="feedbackForm" class="feedback-form" style="display: none;">
            <h3>Feedback</h3>
            <input type="text" placeholder="Your Name" required>
            <textarea placeholder="Your Feedback" required></textarea>
            <button type="submit">Send Feedback</button>
        </div>
    </form>
</div>

<script>
    function toggleForms() {
        var formType = document.getElementById('formType').value;
        if (formType === 'contact') {
            document.getElementById('contactForm').style.display = 'block';
            document.getElementById('feedbackForm').style.display = 'none';
        } else if (formType === 'feedback') {
            document.getElementById('contactForm').style.display = 'none';
            document.getElementById('feedbackForm').style.display = 'block';
        }
    }
</script>

</body>
</html>
