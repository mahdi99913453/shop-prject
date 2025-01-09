## Hey

 **يا أخوتي السلام عليكم**
 **Welcome to my simple project this is a simple shop front end**
  1. if you want to download this projet dont download here is the code:

<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>متجر إلكتروني عصري</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-color: #f1f1f1;
            color: #333;
        }

        header {
            background-color: #232f3e;
            color: white;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            margin: 0;
        }

        nav ul {
            list-style: none;
            display: flex;
            margin: 0;
            padding: 0;
            gap: 1rem;
        }

        nav a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            padding: 0.5rem 1rem;
            transition: background-color 0.3s;
        }

        nav a:hover {
            background-color: #37475a;
            border-radius: 5px;
        }

        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 1rem;
        }

        .products {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            justify-content: center;
        }

        .product {
            background: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 1rem;
            text-align: center;
            width: 300px;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .product:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .product img {
            max-width: 100%;
            border-radius: 8px;
            margin-bottom: 1rem;
        }

        .product h3 {
            font-size: 1.4rem;
            margin: 0.5rem 0;
        }

        .product p {
            color: #555;
            font-size: 1rem;
        }

        .product button {
            background-color: #ff9900;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s;
        }

        .product button:hover {
            background-color: #e68a00;
        }

        .cart {
            margin-top: 2rem;
            text-align: center;
            background: #fff;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .cart h2 {
            margin-bottom: 1rem;
        }

        .cart ul {
            list-style: none;
            padding: 0;
            margin: 1rem 0;
        }

        .cart li {
            margin-bottom: 0.5rem;
        }

        .cart button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s;
        }

        .cart button:hover {
            background-color: #0056b3;
        }

        .payment-form {
            margin-top: 2rem;
            background: #fff;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            width: 400px;
            margin: 2rem auto;
        }

        .payment-form input {
            width: 100%;
            padding: 1rem;
            margin: 0.5rem 0;
            border-radius: 4px;
            border: 1px solid #ddd;
            font-size: 1rem;
        }

        .payment-form button {
            width: 100%;
            padding: 1rem;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 1.2rem;
        }

        .payment-form button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <header>
        <h1>متجر عصري</h1>
        <nav>
            <ul>
                <li><a href="#products">المنتجات</a></li>
                <li><a href="#cart">سلة المشتريات</a></li>
                <li><a href="#payment">الدفع</a></li>
            </ul>
        </nav>
    </header>

    <div class="container">
        <section id="products" class="products">
            <!-- منتج 1 -->
            <div class="product" data-name="هاتف سامسونج جالاكسي" data-price="15000">
                <img src="clipboard.png" alt="هاتف سامسونج جالاكسي">
                <h3>هاتف سامسونج جالاكسي</h3>
                <p>السعر: 15000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 2 -->
            <div class="product" data-name="لابتوب ديل" data-price="25000">
                <img src="clipboard.png" alt="لابتوب ديل">
                <h3>لابتوب ديل</h3>
                <p>السعر: 25000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 3 -->
            <div class="product" data-name="سماعات بلوتوث" data-price="5000">
                <img src="clipboard.png" alt="سماعات بلوتوث">
                <h3>سماعات بلوتوث</h3>
                <p>السعر: 5000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 4 -->
            <div class="product" data-name="كاميرا كانون" data-price="18000">
                <img src="clipboard.png" alt="كاميرا كانون">
                <h3>كاميرا كانون</h3>
                <p>السعر: 18000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 5 -->
            <div class="product" data-name="ساعة ذكية" data-price="8000">
                <img src="clipboard.png" alt="ساعة ذكية">
                <h3>ساعة ذكية</h3>
                <p>السعر: 8000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 6 -->
            <div class="product" data-name="شاحن لاسلكي" data-price="2000">
                <img src="clipboard.png" alt="شاحن لاسلكي">
                <h3>شاحن لاسلكي</h3>
                <p>السعر: 2000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 7 -->
            <div class="product" data-name="مفاتيح مدمجة" data-price="1200">
                <img src="clipboard.png" alt="مفاتيح مدمجة">
                <h3>مفاتيح مدمجة</h3>
                <p>السعر: 1200 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
            <!-- منتج 8 -->
            <div class="product" data-name="تابلت أبل" data-price="30000">
                <img src="clipboard.png" alt="تابلت أبل">
                <h3>تابلت أبل</h3>
                <p>السعر: 30000 دينار</p>
                <button onclick="addToCart(this)">أضف إلى السلة</button>
            </div>
        </section>

        <section id="cart" class="cart">
            <h2>سلة المشتريات</h2>
            <ul id="cart-items"></ul>
            <p id="total-price">الإجمالي: 0 دينار</p>
            <button id="checkout-btn" onclick="checkout()">ادفع الآن</button>
        </section>

        <!-- واجهة الدفع -->
        <section id="payment" class="payment-form" style="display: none;">
            <h2>إتمام الدفع</h2>
            <input type="text" placeholder="رقم البطاقة" id="card-number" required>
            <input type="text" placeholder="تاريخ انتهاء البطاقة" id="expiry-date" required>
            <input type="text" placeholder="رمز الأمان" id="cvv" required>
            <button onclick="processPayment()">دفع</button>
        </section>
    </div>

    <script>
        const cart = [];
        const cartItems = document.getElementById("cart-items");
        const totalPrice = document.getElementById("total-price");
        const paymentSection = document.getElementById("payment");

        function addToCart(button) {
            const product = button.parentElement;
            const name = product.getAttribute("data-name");
            const price = parseInt(product.getAttribute("data-price"));

            cart.push({ name, price });
            updateCart();
        }

        function updateCart() {
            cartItems.innerHTML = "";
            let total = 0;

            cart.forEach(item => {
                const li = document.createElement("li");
                li.textContent = `${item.name} - ${item.price} دينار`;
                cartItems.appendChild(li);
                total += item.price;
            });

            totalPrice.textContent = `الإجمالي: ${total} دينار`;
        }

        function checkout() {
            if (cart.length === 0) {
                alert("السلة فارغة! أضف منتجات قبل الدفع.");
                return;
            }

            paymentSection.style.display = "block";
        }

        function processPayment() {
            const cardNumber = document.getElementById("card-number").value;
            const expiryDate = document.getElementById("expiry-date").value;
            const cvv = document.getElementById("cvv").value;

            if (cardNumber && expiryDate && cvv) {
                alert("تمت معالجة الدفع بنجاح!");
                paymentSection.style.display = "none";
            } else {
                alert("يرجى ملء جميع الحقول.");
            }
        }
    </script>
</body>
</html>

