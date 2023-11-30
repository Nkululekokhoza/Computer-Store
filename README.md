# Computer-Store
This is a computer store to sell gadgets online
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Computer Store</title>
    <style>
        /* Add your CSS styles here */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: white;
            padding: 1em;
            text-align: center;
        }

        section {
            padding: 20px;
        }

        .product {
            border: 1px solid #ccc;
            padding: 10px;
            margin: 10px;
            text-align: center;
            background-color: white;
        }
    </style>
</head>
<body>

    <header>
        <h1>Computer Store</h1>
    </header>

    <section>
        <div class="product" id="product1">
            <img src="laptop.jpg" alt="Laptop">
            <h2>Laptop</h2>
            <p>Powerful laptop for all your needs.</p>
            <button onclick="addToCart('Laptop', 999.99)">Add to Cart</button>
        </div>

        <!-- Add more products as needed -->
    </section>

    <section>
        <h2>Your Cart</h2>
        <ul id="cart"></ul>
    </section>

    <script>
        // JavaScript functions
        function addToCart(productName, price) {
            var cart = document.getElementById('cart');
            var newItem = document.createElement('li');
            newItem.textContent = productName + ' - $' + price;
            cart.appendChild(newItem);
        }
    </script>

</body>
</html>
