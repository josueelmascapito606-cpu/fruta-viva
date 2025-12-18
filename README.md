<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Fruta Viva | Fruta Deshidratada Natural</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        body {
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
            background-color: #fafafa;
            color: #333;
        }

        header {
            background-color: #2e7d32;
            color: white;
            padding: 20px;
            text-align: center;
        }

        header h1 {
            margin: 0;
        }

        nav {
            background-color: #1b5e20;
            display: flex;
            justify-content: center;
            padding: 10px;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }

        nav a:hover {
            text-decoration: underline;
        }

        .hero {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)),
                        url("https://images.unsplash.com/photo-1587049352846-4a222e784d38");
            background-size: cover;
            background-position: center;
            color: white;
            padding: 80px 20px;
            text-align: center;
        }

        .hero h2 {
            font-size: 36px;
        }

        .container {
            max-width: 1100px;
            margin: auto;
            padding: 40px 20px;
        }

        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .product {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
            padding: 20px;
            text-align: center;
        }

        .product img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 6px;
        }

        .product h3 {
            margin: 15px 0 10px;
        }

        .price {
            color: #2e7d32;
            font-size: 20px;
            font-weight: bold;
        }

        button {
            background-color: #2e7d32;
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }

        button:hover {
            background-color: #1b5e20;
        }

        .about {
            background-color: #f1f8e9;
            border-radius: 8px;
            padding: 30px;
        }

        footer {
            background-color: #1b5e20;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }

        .cart {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background-color: #2e7d32;
            color: white;
            padding: 15px 20px;
            border-radius: 30px;
            font-weight: bold;
        }
    </style>
</head>
<body>

<header>
    <h1>🍍 Fruta Viva</h1>
    <p>Fruta deshidratada 100% natural</p>
</header>

<nav>
    <a href="#productos">Productos</a>
    <a href="#nosotros">Nosotros</a>
    <a href="#contacto">Contacto</a>
</nav>

<section class="hero">
    <h2>Sabores naturales, energía real</h2>
    <p>Sin azúcar añadida • Sin conservantes • Hecho artesanalmente</p>
</section>

<div class="container" id="productos">
    <h2>Nuestros Productos</h2>

    <div class="products">
        <div class="product">
            <img src="https://images.unsplash.com/photo-1576402187878-974f70c890a5">
            <h3>Manzana Deshidratada</h3>
            <p>Rodajas crujientes y dulces</p>
            <div class="price">$5.00</div>
            <button onclick="addToCart()">Agregar al carrito</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1601004890684-d8cbf643f5f2">
            <h3>Mango Deshidratado</h3>
            <p>Suave, tropical y natural</p>
            <div class="price">$6.50</div>
            <button onclick="addToCart()">Agregar al carrito</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1592921870789-04563d55041c">
            <h3>Banana Deshidratada</h3>
            <p>Ideal para snacks saludables</p>
            <div class="price">$4.50</div>
            <button onclick="addToCart()">Agregar al carrito</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1615485290382-441e4d049cb5">
            <h3>Piña Deshidratada</h3>
            <p>Ácida y dulce al mismo tiempo</p>
            <div class="price">$6.00</div>
            <button onclick="addToCart()">Agregar al carrito</button>
        </div>
    </div>
</div>

<div class="container" id="nosotros">
    <h2>Sobre Nosotros</h2>
    <div class="about">
        <p>
            En <strong>Fruta Viva</strong> nos dedicamos a deshidratar frutas frescas
            de productores locales, conservando su sabor, nutrientes y textura.
            Nuestro proceso es artesanal y cuidadoso, pensado para personas que
            buscan una alimentación más natural y consciente.
        </p>
    </div>
</div>

<div class="container" id="contacto">
    <h2>Contacto</h2>
    <p>Email: contacto@frutaviva.com</p>
    <p>WhatsApp: +34 600 123 456</p>
</div>

<footer>
    <p>© 2025 Fruta Viva - Todos los derechos reservados</p>
</footer>

<div class="cart" id="cart">
    🛒 Carrito: <span id="count">0</span>
</div>

<script>
    let cartCount = 0;

    function addToCart() {
        cartCount++;
        document.getElementById("count").innerText = cartCount;
        alert("Producto agregado al carrito");
    }
</script>

</body>
</html>
