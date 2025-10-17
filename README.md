# akvarios
Российские Очистные Сооружения является одним из ведущих производителей на рынке локальных очистных сооружений в России и ближнем зарубежье.  НПО "РОС" занимается проектированием, производством, строительством, согласование, обслуживанием и реконструкцией очистных сооружений хозяйственно-бытовых сточных вод.

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Akvalos - Интернет-магазин аквариумов и товаров для аквариумистики</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Header Styles */
        .header-top {
            background-color: #f8f9fa;
            padding: 10px 0;
            border-bottom: 1px solid #eaeaea;
            font-size: 14px;
        }
        
        .header-top .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .contact-info span {
            margin-right: 20px;
        }
        
        .contact-info i {
            color: #0066cc;
            margin-right: 5px;
        }
        
        .user-links a {
            margin-left: 15px;
            text-decoration: none;
            color: #555;
        }
        
        .user-links a:hover {
            color: #0066cc;
        }
        
        .main-header {
            background-color: white;
            padding: 15px 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 28px;
            font-weight: 700;
            color: #0066cc;
            display: flex;
            align-items: center;
        }
        
        .logo i {
            margin-right: 10px;
            font-size: 32px;
        }
        
        .search-bar {
            flex-grow: 1;
            max-width: 500px;
            margin: 0 30px;
            position: relative;
        }
        
        .search-bar input {
            width: 100%;
            padding: 12px 20px;
            border: 1px solid #ddd;
            border-radius: 30px;
            font-size: 16px;
            outline: none;
        }
        
        .search-bar button {
            position: absolute;
            right: 5px;
            top: 5px;
            background: #0066cc;
            color: white;
            border: none;
            border-radius: 30px;
            padding: 7px 20px;
            cursor: pointer;
        }
        
        .header-actions {
            display: flex;
            align-items: center;
        }
        
        .header-action {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-left: 20px;
            cursor: pointer;
        }
        
        .header-action i {
            font-size: 22px;
            color: #0066cc;
            margin-bottom: 5px;
        }
        
        .header-action span {
            font-size: 12px;
            color: #555;
        }
        
        .cart-count {
            background: #ff4d4d;
            color: white;
            border-radius: 50%;
            width: 18px;
            height: 18px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            position: absolute;
            top: -5px;
            right: -5px;
        }
        
        /* Navigation */
        .main-nav {
            background-color: #0066cc;
        }
        
        .nav-menu {
            display: flex;
            list-style: none;
        }
        
        .nav-menu li {
            position: relative;
        }
        
        .nav-menu a {
            display: block;
            padding: 15px 20px;
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: background-color 0.3s;
        }
        
        .nav-menu a:hover {
            background-color: #0052a3;
        }
        
        .nav-menu li:hover .submenu {
            display: block;
        }
        
        .submenu {
            display: none;
            position: absolute;
            top: 100%;
            left: 0;
            background: white;
            min-width: 200px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            z-index: 1000;
        }
        
        .submenu a {
            color: #333;
            padding: 12px 20px;
            border-bottom: 1px solid #eee;
        }
        
        .submenu a:hover {
            background: #f5f7fa;
            color: #0066cc;
        }
        
        /* Banner */
        .banner {
            background: linear-gradient(rgba(0, 102, 204, 0.8), rgba(0, 102, 204, 0.9)), url('https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1200&q=80') no-repeat center center;
            background-size: cover;
            color: white;
            text-align: center;
            padding: 80px 20px;
            margin-bottom: 40px;
        }
        
        .banner h1 {
            font-size: 42px;
            margin-bottom: 20px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.3);
        }
        
        .banner p {
            font-size: 20px;
            margin-bottom: 30px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .btn {
            display: inline-block;
            background-color: #ff9900;
            color: white;
            padding: 14px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            font-size: 16px;
            transition: all 0.3s;
            box-shadow: 0 4px 10px rgba(255, 153, 0, 0.3);
        }
        
        .btn:hover {
            background-color: #e68a00;
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(255, 153, 0, 0.4);
        }
        
        /* Categories */
        .categories {
            padding: 40px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 32px;
            color: #0066cc;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            display: block;
            width: 80px;
            height: 3px;
            background: #ff9900;
            margin: 10px auto;
        }
        
        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }
        
        .category-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s, box-shadow 0.3s;
            text-align: center;
        }
        
        .category-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .category-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .category-card h3 {
            padding: 20px 15px;
            font-size: 20px;
            color: #333;
        }
        
        /* Products */
        .products {
            padding: 40px 0;
            background-color: #fff;
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 25px;
        }
        
        .product-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
            position: relative;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-badge {
            position: absolute;
            top: 10px;
            left: 10px;
            background: #ff4d4d;
            color: white;
            padding: 5px 10px;
            border-radius: 3px;
            font-size: 12px;
            font-weight: bold;
        }
        
        .product-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        
        .product-info {
            padding: 15px;
        }
        
        .product-title {
            font-size: 16px;
            margin-bottom: 10px;
            height: 40px;
            overflow: hidden;
        }
        
        .product-price {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-top: 15px;
        }
        
        .price {
            font-weight: bold;
            color: #0066cc;
            font-size: 18px;
        }
        
        .old-price {
            text-decoration: line-through;
            color: #999;
            font-size: 14px;
            margin-left: 5px;
        }
        
        .add-to-cart {
            background: #0066cc;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 8px 15px;
            cursor: pointer;
            transition: background 0.3s;
        }
        
        .add-to-cart:hover {
            background: #0052a3;
        }
        
        /* Features */
        .features {
            padding: 60px 0;
            background-color: #f8f9fa;
        }
        
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .feature {
            text-align: center;
            padding: 30px 20px;
        }
        
        .feature i {
            font-size: 40px;
            color: #0066cc;
            margin-bottom: 20px;
        }
        
        .feature h3 {
            margin-bottom: 15px;
            color: #333;
        }
        
        .feature p {
            color: #666;
        }
        
        /* Footer */
        footer {
            background-color: #2c3e50;
            color: white;
            padding: 60px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            margin-bottom: 25px;
            font-size: 18px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-column h3:after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 40px;
            height: 2px;
            background: #ff9900;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 12px;
        }
        
        .footer-column a {
            color: #bdc3c7;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column a:hover {
            color: white;
        }
        
        .social-links {
            display: flex;
            margin-top: 20px;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 36px;
            height: 36px;
            background: rgba(255,255,255,0.1);
            border-radius: 50%;
            margin-right: 10px;
            transition: background 0.3s;
        }
        
        .social-links a:hover {
            background: #0066cc;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: #bdc3c7;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 992px) {
            .header-content {
                flex-wrap: wrap;
            }
            
            .search-bar {
                order: 3;
                max-width: 100%;
                margin: 15px 0 0;
            }
            
            .nav-menu {
                flex-wrap: wrap;
            }
        }
        
        @media (max-width: 768px) {
            .banner h1 {
                font-size: 32px;
            }
            
            .banner p {
                font-size: 18px;
            }
            
            .section-title {
                font-size: 28px;
            }
            
            .category-grid, .product-grid {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            }
        }
        
        @media (max-width: 576px) {
            .header-top .container {
                flex-direction: column;
                text-align: center;
            }
            
            .contact-info {
                margin-bottom: 10px;
            }
            
            .category-grid, .product-grid {
                grid-template-columns: 1fr 1fr;
            }
            
            .feature-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header Top -->
    <div class="header-top">
        <div class="container">
            <div class="contact-info">
                <span><i class="fas fa-phone"></i> 8 (800) 123-45-67</span>
                <span><i class="fas fa-envelope"></i> info@akvalos.ru</span>
            </div>
            <div class="user-links">
                <a href="#"><i class="fas fa-user"></i> Личный кабинет</a>
                <a href="#"><i class="fas fa-heart"></i> Избранное</a>
                <a href="#"><i class="fas fa-shopping-cart"></i> Корзина</a>
            </div>
        </div>
    </div>

    <!-- Main Header -->
    <header class="main-header">
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-fish"></i>
                    AKVALOS
                </div>
                <div class="search-bar">
                    <input type="text" placeholder="Поиск товаров...">
                    <button><i class="fas fa-search"></i></button>
                </div>
                <div class="header-actions">
                    <div class="header-action">
                        <i class="fas fa-phone-alt"></i>
                        <span>Позвонить</span>
                    </div>
                    <div class="header-action">
                        <i class="fas fa-heart"></i>
                        <span>Избранное</span>
                    </div>
                    <div class="header-action" style="position: relative;">
                        <i class="fas fa-shopping-cart"></i>
                        <span>Корзина</span>
                        <div class="cart-count">3</div>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <!-- Navigation -->
    <nav class="main-nav">
        <div class="container">
            <ul class="nav-menu">
                <li><a href="#">Главная</a></li>
                <li>
                    <a href="#">Аквариумы <i class="fas fa-chevron-down"></i></a>
                    <ul class="submenu">
                        <li><a href="#">Пресноводные аквариумы</a></li>
                        <li><a href="#">Морские аквариумы</a></li>
                        <li><a href="#">Аквариумы для креветок</a></li>
                        <li><a href="#">Аквариумы-террариумы</a></li>
                    </ul>
                </li>
                <li><a href="#">Рыбки</a></li>
                <li><a href="#">Растения</a></li>
                <li><a href="#">Оборудование</a></li>
                <li><a href="#">Корма</a></li>
                <li><a href="#">Акции</a></li>
                <li><a href="#">Доставка</a></li>
                <li><a href="#">Контакты</a></li>
            </ul>
        </div>
    </nav>

    <!-- Banner -->
    <section class="banner">
        <div class="container">
            <h1>Мир аквариумистики в одном месте</h1>
            <p>Широкий выбор аквариумов, рыбок и аксессуаров для вашего хобби. Качество, которое вы заслуживаете!</p>
            <a href="#" class="btn">Перейти в каталог</a>
        </div>
    </section>

    <!-- Categories -->
    <section class="categories">
        <div class="container">
            <h2 class="section-title">Категории товаров</h2>
            <div class="category-grid">
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Аквариумы">
                    <h3>Аквариумы</h3>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1522065893269-6fd20f6d7438?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Рыбки">
                    <h3>Рыбки</h3>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1560574188-6a6774965120?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Растения">
                    <h3>Аквариумные растения</h3>
                </div>
                <div class="category-card">
                    <img src="https://images.unsplash.com/photo-1576613109753-27804de2cba8?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Оборудование">
                    <h3>Оборудование</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Products -->
    <section class="products">
        <div class="container">
            <h2 class="section-title">Популярные товары</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-badge">Хит</div>
                    <img src="https://images.unsplash.com/photo-1576808216213-7c64cce424d5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Аквариум 100л">
                    <div class="product-info">
                        <h3 class="product-title">Аквариум прямоугольный 100л с тумбой</h3>
                        <div class="product-price">
                            <div>
                                <span class="price">8 490 ₽</span>
                                <span class="old-price">9 990 ₽</span>
                            </div>
                            <button class="add-to-cart"><i class="fas fa-cart-plus"></i></button>
                        </div>
                    </div>
                </div>
                <div class="product-card">
                    <div class="product-badge">Акция</div>
                    <img src="https://images.unsplash.com/photo-1597848212624-e6d4bd66d381?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Фильтр">
                    <div class="product-info">
                        <h3 class="product-title">Внутренний фильтр Aquael Fan 2 plus</h3>
                        <div class="product-price">
                            <div>
                                <span class="price">2 350 ₽</span>
                            </div>
                            <button class="add-to-cart"><i class="fas fa-cart-plus"></i></button>
                        </div>
                    </div>
                </div>
                <div class="product-card">
                    <img src="https://images.unsplash.com/photo-1576675466969-38eeae4b41f6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Корм">
                    <div class="product-info">
                        <h3 class="product-title">Корм для рыб TetraMin Flakes 100ml</h3>
                        <div class="product-price">
                            <div>
                                <span class="price">650 ₽</span>
                            </div>
                            <button class="add-to-cart"><i class="fas fa-cart-plus"></i></button>
                        </div>
                    </div>
                </div>
                <div class="product-card">
                    <img src="https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=600&q=80" alt="Обогреватель">
                    <div class="product-info">
                        <h3 class="product-title">Обогреватель аквариумный 100Вт с терморегулятором</h3>
                        <div class="product-price">
                            <div>
                                <span class="price">1 290 ₽</span>
                            </div>
                            <button class="add-to-cart"><i class="fas fa-cart-plus"></i></button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Features -->
    <section class="features">
        <div class="container">
            <h2 class="section-title">Почему выбирают нас</h2>
            <div class="feature-grid">
                <div class="feature">
                    <i class="fas fa-shipping-fast"></i>
                    <h3>Быстрая доставка</h3>
                    <p>Доставляем заказы по всей России в кратчайшие сроки</p>
                </div>
                <div class="feature">
                    <i class="fas fa-award"></i>
                    <h3>Гарантия качества</h3>
                    <p>Все товары проходят тщательную проверку перед отправкой</p>
                </div>
                <div class="feature">
                    <i class="fas fa-headset"></i>
                    <h3>Поддержка 24/7</h3>
                    <p>Наши специалисты всегда готовы ответить на ваши вопросы</p>
                </div>
                <div class="feature">
                    <i class="fas fa-hand-holding-usd"></i>
                    <h3>Выгодные цены</h3>
                    <p>Предлагаем конкурентные цены и регулярные акции</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Каталог</h3>
                    <ul>
                        <li><a href="#">Аквариумы</a></li>
                        <li><a href="#">Рыбки</a></li>
                        <li><a href="#">Растения</a></li>
                        <li><a href="#">Оборудование</a></li>
                        <li><a href="#">Корма</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Помощь</h3>
                    <ul>
                        <li><a href="#">Доставка и оплата</a></li>
                        <li><a href="#">Гарантия и возврат</a></li>
                        <li><a href="#">Вопросы и ответы</a></li>
                        <li><a href="#">Статьи и советы</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>О компании</h3>
                    <ul>
                        <li><a href="#">О нас</a></li>
                        <li><a href="#">Контакты</a></li>
                        <li><a href="#">Вакансии</a></li>
                        <li><a href="#">Отзывы</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Контакты</h3>
                    <ul>
                        <li><i class="fas fa-phone"></i> 8 (800) 123-45-67</li>
                        <li><i class="fas fa-envelope"></i> info@akvalos.ru</li>
                        <li><i class="fas fa-map-marker-alt"></i> Москва, ул. Аквариумная, 15</li>
                        <li><i class="fas fa-clock"></i> Пн-Вс 9:00-21:00</li>
                    </ul>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-vk"></i></a>
                        <a href="#"><i class="fab fa-telegram"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-youtube"></i></a>
                    </div>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Akvalos.ru - Интернет-магазин аквариумов и товаров для аквариумистики. Все права защищены.</p>
            </div>
        </div>
    </footer>
</body>
</html>
