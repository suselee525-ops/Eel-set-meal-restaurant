# Eel-set-meal-restaurant
[[Kuse] 鰻牛 現烤鰻魚定食  花蓮日式料理 (1).html](https://github.com/user-attachments/files/26125067/Kuse.1.html)
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>鰻牛 現烤鰻魚定食 | 花蓮日式料理</title>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@400;600;700&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-dark: #1a1410;
            --secondary-dark: #2d2318;
            --accent-gold: #d4af37;
            --accent-orange: #ff6b35;
            --text-light: #f5f5f5;
            --text-gold: #ffd700;
        }

        body {
            font-family: 'Noto Serif TC', serif;
            background-color: var(--primary-dark);
            color: var(--text-light);
            overflow-x: hidden;
        }

        .font-poppins {
            font-family: 'Poppins', sans-serif;
        }

        html {
            scroll-behavior: smooth;
        }

        .hero-section {
            position: relative;
            height: 100vh;
            min-height: 600px;
            background: linear-gradient(rgba(26, 20, 16, 0.7), rgba(26, 20, 16, 0.8)), 
                        url('https://sudachirecipes.com/wp-content/uploads/2022/07/unagi-don-sqr-550x550.jpg') center/cover no-repeat;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }

        .hero-content {
            z-index: 10;
            padding: 20px;
        }

        .restaurant-name {
            font-size: clamp(2.5rem, 6vw, 5rem);
            font-weight: 700;
            color: var(--text-gold);
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.8);
            margin-bottom: 20px;
            letter-spacing: 2px;
        }

        .rating-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 15px;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .stars {
            color: var(--accent-gold);
            font-size: 1.8rem;
            letter-spacing: 3px;
        }

        .rating-text {
            font-size: 1.2rem;
            color: var(--text-light);
            font-family: 'Poppins', sans-serif;
        }

        .nav-bar {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            background: rgba(26, 20, 16, 0.95);
            backdrop-filter: blur(10px);
            padding: 15px 0;
            z-index: 1000;
            transition: all 0.3s ease;
            border-bottom: 1px solid rgba(212, 175, 55, 0.3);
        }

        .nav-bar.scrolled {
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.5);
        }

        .nav-links {
            display: flex;
            justify-content: center;
            gap: 40px;
            list-style: none;
            flex-wrap: wrap;
            padding: 0 20px;
        }

        .nav-links a {
            color: var(--text-light);
            text-decoration: none;
            font-size: 1rem;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--accent-gold);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent-gold);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .section {
            padding: 80px 20px;
            max-width: 1400px;
            margin: 0 auto;
        }

        .section-title {
            font-size: clamp(2rem, 4vw, 3rem);
            color: var(--accent-gold);
            text-align: center;
            margin-bottom: 50px;
            position: relative;
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: var(--accent-orange);
        }

        .announcement-banner {
            background: linear-gradient(135deg, var(--accent-orange), #ff8c5a);
            padding: 25px;
            border-radius: 12px;
            text-align: center;
            margin: 30px auto;
            max-width: 800px;
            box-shadow: 0 8px 24px rgba(255, 107, 53, 0.3);
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.02); }
        }

        .announcement-banner h3 {
            font-size: 1.5rem;
            color: white;
            margin-bottom: 10px;
            font-weight: 700;
        }

        .announcement-banner p {
            font-size: 1.1rem;
            color: white;
        }

        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .menu-card {
            background: var(--secondary-dark);
            border-radius: 16px;
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 2px solid rgba(212, 175, 55, 0.2);
        }

        .menu-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 40px rgba(212, 175, 55, 0.3);
        }

        .menu-card-image {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }

        .menu-card-content {
            padding: 25px;
        }

        .menu-card-title {
            font-size: 1.5rem;
            color: var(--accent-gold);
            margin-bottom: 10px;
            font-weight: 600;
        }

        .menu-card-description {
            color: var(--text-light);
            line-height: 1.6;
            font-size: 1rem;
        }

        .review-card {
            background: var(--secondary-dark);
            padding: 30px;
            border-radius: 12px;
            margin-bottom: 25px;
            border-left: 4px solid var(--accent-gold);
            transition: transform 0.3s ease;
        }

        .review-card:hover {
            transform: translateX(10px);
        }

        .review-stars {
            color: var(--accent-gold);
            font-size: 1.2rem;
            margin-bottom: 10px;
        }

        .review-text {
            color: var(--text-light);
            line-height: 1.8;
            font-size: 1.05rem;
            margin-bottom: 15px;
        }

        .review-author {
            color: var(--accent-orange);
            font-weight: 600;
            font-size: 0.95rem;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .contact-item {
            background: var(--secondary-dark);
            padding: 30px;
            border-radius: 12px;
            text-align: center;
            transition: transform 0.3s ease;
            border: 2px solid rgba(212, 175, 55, 0.2);
        }

        .contact-item:hover {
            transform: scale(1.05);
        }

        .contact-icon {
            font-size: 2.5rem;
            color: var(--accent-gold);
            margin-bottom: 15px;
        }

        .contact-label {
            font-size: 1.1rem;
            color: var(--accent-orange);
            margin-bottom: 10px;
            font-weight: 600;
        }

        .contact-value {
            font-size: 1rem;
            color: var(--text-light);
            line-height: 1.6;
        }

        .contact-value a {
            color: var(--text-light);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .contact-value a:hover {
            color: var(--accent-gold);
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--accent-gold), #ffd700);
            color: var(--primary-dark);
            padding: 15px 40px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            display: inline-block;
            margin-top: 20px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            font-size: 1.1rem;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(212, 175, 55, 0.4);
        }

        .service-badges {
            display: flex;
            gap: 15px;
            justify-content: center;
            margin-top: 20px;
            flex-wrap: wrap;
        }

        .badge {
            background: var(--accent-orange);
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            font-size: 0.95rem;
            font-weight: 500;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }

        .price-range {
            font-size: 1.3rem;
            color: var(--accent-gold);
            font-weight: 600;
            margin-top: 15px;
        }

        .about-content {
            max-width: 900px;
            margin: 0 auto;
            text-align: center;
            line-height: 2;
            font-size: 1.15rem;
            color: var(--text-light);
        }

        .kuse-branding {
            text-align: center;
            padding: 40px 20px;
            background: rgba(45, 35, 24, 0.5);
            margin-top: 60px;
        }

        .kuse-branding a {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            color: var(--text-light);
            text-decoration: none;
            font-size: 0.95rem;
            transition: color 0.3s ease;
        }

        .kuse-branding a:hover {
            color: var(--accent-gold);
        }

        .kuse-branding svg {
            height: 1.2em;
            transition: transform 0.3s ease;
        }

        .kuse-branding a:hover svg {
            transform: scale(1.1);
        }

        @media (max-width: 768px) {
            .nav-links {
                gap: 20px;
                font-size: 0.9rem;
            }

            .section {
                padding: 60px 15px;
            }

            .menu-grid {
                grid-template-columns: 1fr;
            }

            .contact-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <nav class="nav-bar" id="navbar">
        <ul class="nav-links">
            <li><a href="#home">首頁</a></li>
            <li><a href="#about">關於我們</a></li>
            <li><a href="#menu">招牌菜單</a></li>
            <li><a href="#reviews">顧客評價</a></li>
            <li><a href="#contact">聯絡資訊</a></li>
        </ul>
    </nav>

    <section id="home" class="hero-section">
        <div class="hero-content">
            <h1 class="restaurant-name">鰻牛 現烤鰻魚定食</h1>
            <div class="rating-container">
                <div class="stars">★★★★★</div>
                <span class="rating-text font-poppins">4.7 / 5.0 (298則評論)</span>
            </div>
            <p class="price-range font-poppins">NT$ 400 - 600</p>
            <div class="service-badges">
                <span class="badge">🍽️ 內用</span>
                <span class="badge">🚗 外送</span>
            </div>
            <div class="announcement-banner">
                <h3>📢 店休公告</h3>
                <p>2/25-3/3鰻牛店休，3/4開始營業！</p>
            </div>
        </div>
    </section>

    <section id="about" class="section">
        <h2 class="section-title">關於我們</h2>
        <div class="about-content">
            <p>鰻牛現烤鰻魚定食位於花蓮吉安鄉，以新鮮現烤的淡水鰻魚與頂級和牛料理聞名。我們堅持使用最優質的食材，每一道料理都經過廚師精心烹調，呈現最道地的日式風味。</p>
            <br>
            <p>環境優雅舒適，服務親切專業，無論是家庭聚餐或朋友小聚，都能在這裡享受到賓至如歸的用餐體驗。我們的招牌鰻牛海陸套餐，結合了海洋與陸地的頂級美味，讓您一次品嚐雙重享受。</p>
        </div>
    </section>

    <section id="menu" class="section" style="background: rgba(45, 35, 24, 0.3);">
        <h2 class="section-title">招牌菜單</h2>
        <div class="menu-grid">
            <div class="menu-card">
                <img src="https://www.justonecookbook.com/wp-content/uploads/2021/07/Unadon-Eel-Rice-9543-I-1.jpg" alt="現烤鰻魚定食" class="menu-card-image">
                <div class="menu-card-content">
                    <h3 class="menu-card-title">現烤鰻魚定食</h3>
                    <p class="menu-card-description">精選淡水鰻魚，以傳統蒲燒手法現烤，魚肉厚實鮮嫩，搭配特製醬汁，香氣四溢。套餐附贈精緻小菜、味噌湯及季節甜點。</p>
                </div>
            </div>

            <div class="menu-card">
                <img src="https://rimage.savorjapan.com/svj/image/discover_oishii_japan/1224/article_329895_w640z.jpg" alt="頂級和牛料理" class="menu-card-image">
                <div class="menu-card-content">
                    <h3 class="menu-card-title">頂級和牛料理</h3>
                    <p class="menu-card-description">嚴選和牛阪腱，油花分布均勻，肉質軟嫩。提供現烤烤阪腱定食與經典壽喜燒，讓您品嚐和牛的極致美味。</p>
                </div>
            </div>

            <div class="menu-card">
                <img src="https://cdn.media.amplience.net/i/japancentre/recipe-1434-unagi-don-grilled-eel-rice-bowl/Unagi-don-grilled-eel-rice-bowl?$poi$&w=700&h=410&sm=c&fmt=auto" alt="鰻牛海陸套餐" class="menu-card-image">
                <div class="menu-card-content">
                    <h3 class="menu-card-title">鰻牛海陸套餐</h3>
                    <p class="menu-card-description">店內最受歡迎的組合！結合現烤鰻魚與頂級和牛，一次滿足海陸雙重享受。搭配干貝、精緻小菜，最後以芒果冰淇淋完美收尾。</p>
                </div>
            </div>
        </div>
    </section>

    <section id="reviews" class="section">
        <h2 class="section-title">顧客評價</h2>
        <div style="max-width: 900px; margin: 0 auto;">
            <div class="review-card">
                <div class="review-stars">★★★★★</div>
                <p class="review-text">「這次造訪『鰻牛定食』，整體用餐體驗令人驚艷。餐廳主打的鰻魚與和牛組合非常有創意，成功打破了傳統定食的框架，讓人在一份餐點中就能享受海陸雙饗的層次感。」</p>
                <p class="review-author">— 姚璋 (在地嚮導)</p>
            </div>

            <div class="review-card">
                <div class="review-stars">★★★★★</div>
                <p class="review-text">「烤阪腱定食自己烤很容易上手，肉質軟嫩；壽喜燒上桌即食，甜甜醬油香。環境很棒，牛肉鰻魚餐點新鮮，當月壽星另有驚喜❤️推薦👍」</p>
                <p class="review-author">— patrice lin</p>
            </div>

            <div class="review-card">
                <div class="review-stars">★★★★★</div>
                <p class="review-text">「孩子特愛老闆烹飪的鰻魚，炸的很嫩不乾；其他巧手料理的食材，每樣都讓孩子恨不得可以再多一個胃全部塞到肚子裡。環境很乾淨、店員很友善、廚師很專業，能感受到做料理的用心。」</p>
                <p class="review-author">— Zoe Lee</p>
            </div>

            <div class="review-card">
                <div class="review-stars">★★★★★</div>
                <p class="review-text">「套餐的主菜鰻魚，量多又厚實，搭配簡單的配菜和湯，並附加甜點。整體用餐體驗非常滿意，CP值很高！」</p>
                <p class="review-author">— 顧客評論</p>
            </div>
        </div>
    </section>

    <section id="contact" class="section" style="background: rgba(45, 35, 24, 0.3);">
        <h2 class="section-title">聯絡資訊</h2>
        <div class="contact-grid">
            <div class="contact-item">
                <div class="contact-icon">📍</div>
                <div class="contact-label">地址</div>
                <div class="contact-value">973花蓮縣吉安鄉<br>自立路二段23號</div>
            </div>

            <div class="contact-item">
                <div class="contact-icon">📞</div>
                <div class="contact-label">電話</div>
                <div class="contact-value">
                    <a href="tel:038466636">03 846 6636</a>
                </div>
            </div>

            <div class="contact-item">
                <div class="contact-icon">🕐</div>
                <div class="contact-label">營業時間</div>
                <div class="contact-value">11:00 開始營業<br>(請來電確認當日營業狀況)</div>
            </div>

            <div class="contact-item">
                <div class="contact-icon">🗺️</div>
                <div class="contact-label">Google地圖</div>
                <div class="contact-value">
                    <a href="https://www.google.com/maps/search/?api=1&query=973花蓮縣吉安鄉自立路二段23號" target="_blank" class="btn-primary" style="margin-top: 10px;">查看地圖</a>
                </div>
            </div>
        </div>
    </section>

    <div class="kuse-branding">
        <a href="https://kuse.ai" target="_blank">
            made with 
            <svg viewBox="0,0,160,44" xmlns="http://www.w3.org/2000/svg"><path d="m.01,20.65C-.43,8.25,9.3-2.03,22.04.34,34.78,2.72,43.29,8.32,43.29,22.9s-8.66,19.01-22.03,20.3C7.9,44.5.46,33.05.01,20.65z" fill="currentColor"/><path fill-rule="evenodd" clip-rule="evenodd" d="m146.76,7.94c8.07,0,13.24,6.15,13.24,14.58v1.39h-20.75c.45,4.05,3.51,7.37,8.57,7.37,2.62,0,5.73-1.05,7.62-2.94l2.67,3.83c-2.67,2.55-6.62,3.88-10.9,3.88-8.07,0-14.08-5.6-14.08-14.08,0-7.76,5.67-14.02,13.63-14.02zm0,4.77c-5.01,0-7.29,3.83-7.57,7.1h15.13c-.11-3.16-2.28-7.1-7.57-7.1z" fill="currentColor"/><path d="m86.64,24.49c0,4.15,2.39,6.84,6.84,6.84,4.4,0,6.84-2.69,6.84-6.84V8.55h5.37v16.33c0,6.7-4.06,11.14-12.21,11.14-8.21,0-12.21-4.5-12.21-11.09V8.55h5.37v15.94zm32.99-16.55c4.49,0,8.06,1.47,10.6,3.86l-2.59,3.81c-2.05-2-5.28-3.08-8.06-3.08-2.88,0-4.84,1.37-4.84,3.32,0,1.91,2.64,2.54,5.81,3.27,4.59,1.08,10.26,2.4,10.26,8.46,0,4.94-3.76,8.41-11.14,8.41-4.98,0-8.94-1.76-11.24-4.11l2.54-4.11c1.86,1.91,5.18,3.67,8.84,3.67,3.91,0,5.57-1.66,5.57-3.62,0-2.3-2.88-2.98-6.21-3.76-4.54-1.08-9.87-2.3-9.87-8.06,0-4.5,4.2-8.06,10.31-8.06zM60.79,20.82,71.44,8.55h6.5L66.46,21.26,78.82,35.44h-6.5l-9.28-11.1-2.25,2.49v8.6h-5.33V8.55h5.33v12.27z" fill="currentColor"/></svg>
        </a>
    </div>

    <script>
        const navbar = document.getElementById(`navbar`);
        
        window.addEventListener(`scroll`, () => {
            if (window.scrollY > 100) {
                navbar.classList.add(`scrolled`);
            } else {
                navbar.classList.remove(`scrolled`);
            }
        });

        document.querySelectorAll(`a[href^="#"]`).forEach(anchor => {
            anchor.addEventListener(`click`, function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute(`href`));
                if (target) {
                    const offsetTop = target.offsetTop - 60;
                    window.scrollTo({
                        top: offsetTop,
                        behavior: `smooth`
                    });
                }
            });
        });

        const observerOptions = {
            threshold: 0.1,
            rootMargin: `0px 0px -100px 0px`
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = `1`;
                    entry.target.style.transform = `translateY(0)`;
                }
            });
        }, observerOptions);

        document.querySelectorAll(`.menu-card, .review-card, .contact-item`).forEach(el => {
            el.style.opacity = `0`;
            el.style.transform = `translateY(30px)`;
            el.style.transition = `opacity 0.6s ease, transform 0.6s ease`;
            observer.observe(el);
        });
    </script>

    <script src="https://cdn.kuse.ai/sdk.prd.js"></script>
</body>
</html>
