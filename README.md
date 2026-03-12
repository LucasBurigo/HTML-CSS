file:///C:/Users/natha/OneDrive/Documentos/Estudos/html-css/exercícios/exercício%20018/teste%20pizzaria/index.html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pizzaria Delícia</title>
    <style>
        /* Reset e estilos gerais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
        }
        
        /* Cabeçalho */
        header {
            background-color: #d32f2f;
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .logo {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 10px;
        }
        
        /* Navegação */
        nav {
            background-color: #b71c1c;
            padding: 15px 0;
        }
        
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
        }
        
        nav ul li {
            margin: 0 15px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #ffccbc;
        }
        
        /* Banner */
        .banner {
            height: 400px;
            background-image: url('https://example.com/pizza-banner.jpg');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
            position: relative;
        }
        
        .banner::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.5);
        }
        
        .banner-content {
            position: relative;
            z-index: 1;
        }
        
        .banner h1 {
            font-size: 3rem;
            margin-bottom: 20px;
        }
        
        .banner p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: #d32f2f;
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #b71c1c;
        }
        
        /* Seção de cardápio */
        .menu {
            padding: 60px 20px;
            text-align: center;
        }
        
        .menu h2 {
            font-size: 2.5rem;
            margin-bottom: 40px;
            color: #d32f2f;
        }
        
        .pizzas {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }
        
        .pizza-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .pizza-card:hover {
            transform: translateY(-10px);
        }
        
        .pizza-img {
            height: 200px;
            width: 100%;
            object-fit: cover;
        }
        
        .pizza-info {
            padding: 20px;
        }
        
        .pizza-info h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }
        
        .pizza-info p {
            color: #666;
            margin-bottom: 15px;
        }
        
        .price {
            font-size: 1.3rem;
            font-weight: bold;
            color: #d32f2f;
        }
        
        /* Rodapé */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 30px 20px;
            margin-top: 50px;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }
        
        .footer-section {
            flex: 1;
            min-width: 250px;
            margin-bottom: 20px;
        }
        
        .footer-section h3 {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: #d32f2f;
        }
        
        .social-icons a {
            color: white;
            margin: 0 10px;
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-icons a:hover {
            color: #ffccbc;
        }
        
        .copyright {
            border-top: 1px solid #555;
            padding-top: 20px;
        }
        
        /* Responsivo */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 5px 0;
            }
            
            .banner h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">Pizzaria Delícia</div>
        <p>Desde 1985 servindo as melhores pizzas da cidade</p>
    </header>
    
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Cardápio</a></li>
            <li><a href="#">Promoções</a></li>
            <li><a href="#">Sobre Nós</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </nav>
    
    <section class="banner">
        <div class="banner-content">
            <h1>As Melhores Pizzas Artesanais</h1>
            <p>Feitas com ingredientes frescos e selecionados</p>
            <a href="#" class="btn">Peça Agora</a>
        </div>
    </section>
    
    <section class="menu">
        <h2>Nosso Cardápio</h2>
        
        <div class="pizzas">
            <!-- Pizza 1 -->
            <div class="pizza-card">
                <img src="https://example.com/pizza-margherita.jpg" alt="Pizza Margherita" class="pizza-img">
                <div class="pizza-info">
                    <h3>Margherita</h3>
                    <p>Molho de tomate, mussarela, manjericão fresco e azeite</p>
                    <div class="price">R$ 45,90</div>
                </div>
            </div>
            
            <!-- Pizza 2 -->
            <div class="pizza-card">
                <img src="https://example.com/pizza-calabresa.jpg" alt="Pizza Calabresa" class="pizza-img">
                <div class="pizza-info">
                    <h3>Calabresa</h3>
                    <p>Molho de tomate, mussarela, calabresa fatiada e cebola</p>
                    <div class="price">R$ 49,90</div>
                </div>
            </div>
            
            <!-- Pizza 3 -->
            <div class="pizza-card">
                <img src="https://example.com/pizza-portuguesa.jpg" alt="Pizza Portuguesa" class="pizza-img">
                <div class="pizza-info">
                    <h3>Portuguesa</h3>
                    <p>Molho de tomate, mussarela, presunto, ovos, cebola e azeitonas</p>
                    <div class="price">R$ 52,90</div>
                </div>
            </div>
            
            <!-- Pizza 4 -->
            <div class="pizza-card">
                <img src="https://example.com/pizza-frango-catupiry.jpg" alt="Pizza Frango com Catupiry" class="pizza-img">
                <div class="pizza-info">
                    <h3>Frango com Catupiry</h3>
                    <p>Molho de tomate, mussarela, frango desfiado e catupiry</p>
                    <div class="price">R$ 55,90</div>
                </div>
            </div>
            
            <!-- Pizza 5 -->
            <div class="pizza-card">
                <img src="https://example.com/pizza-quatro-queijos.jpg" alt="Pizza Quatro Queijos" class="pizza-img">
                <div class="pizza-info">
                    <h3>Quatro Queijos</h3>
                    <p>Molho de tomate, mussarela, provolone, parmesão e gorgonzola</p>
                    <div class="price">R$ 58,90</div>
                </div>
            </div>
            
            <!-- Pizza 6 -->
            <div class="pizza-card">
                <img src="https://example.com/pizza-pepperoni.jpg" alt="Pizza Pepperoni" class="pizza-img">
                <div class="pizza-info">
                    <h3>Pepperoni</h3>
                    <p>Molho de tomate, mussarela e pepperoni</p>
                    <div class="price">R$ 54,90</div>
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>Horário de Funcionamento</h3>
                <p>Terça a Domingo</p>
                <p>18:00 - 23:00</p>
            </div>
            
            <div class="footer-section">
                <h3>Endereço</h3>
                <p>Rua das Pizzas, 123</p>
                <p>Centro - Sua Cidade</p>
            </div>
            
            <div class="footer-section">
                <h3>Contato</h3>
                <p>(11) 1234-5678</p>
                <p>contato@pizzariadelicia.com.br</p>
                <div class="social-icons">
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
        </div>
        
        <div class="copyright">
            <p>&copy; 2023 Pizzaria Delícia. Todos os direitos reservados.</p>
        </div>
    </footer>
    
    <!-- Ícones do Font Awesome (adicione este link no head para os ícones funcionarem) -->
    <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
</body>
</html>
