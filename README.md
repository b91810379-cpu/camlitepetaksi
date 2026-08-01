<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Çamlıtepe Taksi - Batman 7/24 Güvenli Ulaşım</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        header {
            background: #ffcc00;
            color: #111;
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 8px rgba(0,0,0,0.2);
        }
        .container {
            width: 90%;
            max-width: 1100px;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 24px;
            font-weight: bold;
            text-transform: uppercase;
        }
        .phone-header {
            background: #111;
            color: #ffcc00;
            padding: 10px 20px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            font-size: 18px;
            transition: 0.3s;
        }
        .phone-header:hover {
            background: #333;
        }
        /* Slider Alanı */
        .slider {
            width: 100%;
            height: 450px;
            position: relative;
            overflow: hidden;
        }
        .slide {
            width: 100%;
            height: 100%;
            position: absolute;
            top: 0;
            left: 100%;
            background-size: cover;
            background-position: center;
            transition: left 1s ease-in-out;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .slide.active {
            left: 0;
        }
        .slide-content {
            background: rgba(0,0,0,0.6);
            color: #ffcc00;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
        }
        .slide-content h1 {
            font-size: 48px;
            margin-bottom: 10px;
        }
        .slide-content p {
            font-size: 20px;
            color: #fff;
        }
        /* Hero Alanı (Slider yerine geçecek) */
        .hero-alt {
            background: linear-gradient(135deg, #111 0%, #444 100%);
            color: #ffcc00;
            padding: 60px 20px;
            text-align: center;
        }
        .hero-alt h2 {
            font-size: 36px;
            margin-bottom: 10px;
        }
        .hero-alt p {
            font-size: 18px;
            color: #fff;
            max-width: 600px;
            margin: 0 auto 20px auto;
        }
        .features {
            padding: 60px 20px;
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            background: #fff;
            gap: 30px;
        }
        .feature-box {
            flex-basis: 30%;
            min-width: 280px;
            padding: 30px;
            text-align: center;
            border: 1px solid #eee;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
            transition: 0.3s;
        }
        .feature-box:hover {
            transform: translateY(-5px);
            border-color: #ffcc00;
        }
        .feature-box h3 {
            margin-bottom: 15px;
            color: #111;
            font-size: 22px;
        }
        .feature-box p {
            color: #666;
        }
        footer {
            background: #111;
            color: #888;
            text-align: center;
            padding: 30px;
            margin-top: 50px;
        }
        .footer-phone {
            font-size: 24px;
            color: #ffcc00;
            font-weight: bold;
            margin-top: 10px;
            display: block;
            text-decoration: none;
        }
        .fixed-call {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #ffcc00;
            color: #111;
            padding: 15px 25px;
            border-radius: 50px;
            font-weight: bold;
            text-decoration: none;
            box-shadow: 0 4px 15px rgba(0,0,0,0.4);
            z-index: 1000;
            font-size: 18px;
        }
    </style>
</head>
<body>

    <header>
        <div class="container">
            <div class="logo">Çamlıtepe Taksi</div>
            <a href="tel:05306378449" class="phone-header">📞 0530 637 84 49</a>
        </div>
    </header>

    <!-- Hareketli Slider (Fiat Linea Taksi Görselleri) -->
    <section class="slider">
        <!-- Resim 1: Taksi Önden -->
        <div class="slide active" style="background-image: url('https://images.unsplash.com/photo-1597420860078-115e2f03d08c?auto=format&fit=crop&w=1200&q=80');">
            <div class="slide-content">
                <h1>Batman Çamlıtepe Taksi</h1>
                <p>7/24 Hızlı ve Güvenli Ulaşım</p>
            </div>
        </div>
        <!-- Resim 2: Taksi Yolda -->
        <div class="slide" style="background-image: url('https://images.unsplash.com/photo-1564190937480-6f6b89d86853?auto=format&fit=crop&w=1200&q=80');">
            <div class="slide-content">
                <h1>Konforlu Araçlarımızla</h1>
                <p>Dilediğiniz Yere Hemen Gelelim</p>
            </div>
        </div>
         <!-- Resim 3: Hizmet -->
        <div class="slide" style="background-image: url('https://images.unsplash.com/photo-1615789646145-2a26e8e93502?auto=format&fit=crop&w=1200&q=80');">
            <div class="slide-content">
                <h1>En Yakın Taksi</h1>
                <p>Hemen Arayın: 0530 637 84 49</p>
            </div>
        </div>
    </section>

    <!-- Orta Bilgi Alanı -->
    <section class="hero-alt">
        <h2>Batman Genelinde 7/24 Hizmetinizdeyiz</h2>
        <p>İster Çamlıtepe'de olun, ister Batman'in diğer ucunda. Deneyimli şoförlerimiz ve konforlu Fiat Linea taksilerimizle 7 gün 24 saat emrinizdeyiz. Güvenliğiniz ve konforunuz bizim için önceliklidir.</p>
        <a href="tel:05306378449" class="phone-header" style="display: inline-block; margin-top: 10px;">📞 0530 637 84 49</a>
    </section>

    <!-- Özellikler Kutuları -->
    <section class="features">
        <div class="feature-box">
            <h3>🚖 7/24 Kesintisiz Ulaşım</h3>
            <p>Günün her saati, gece veya gündüz, Batman'de taksi ihtiyacınız için bizi arayabilirsiniz.</p>
        </div>
        <div class="feature-box">
            <h3>🛡️ Güvenli ve Konforlu</h3>
            <p>Bakımlı ve temiz araçlarımızla, deneyimli şoförler eşliğinde huzurlu bir yolculuk yapın.</p>
        </div>
        <div class="feature-box">
            <h3>⚡ Hızlı ve Zamanında</h3>
            <p>Konumunuza en yakın taksimizi yönlendiriyor, sizi bekletmeden adresinize ulaşıyoruz.</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Çamlıtepe Taksi - Tüm hakları saklıdır.</p>
        <a href="tel:05306378449" class="footer-phone">0530 637 84 49</a>
    </footer>

    <!-- Sabit Arama Butonu (Telefonda Hep Görünür) -->
    <a href="tel:05306378449" class="fixed-call">📞 Hemen Ara</a>

    <!-- Slider JavaScript Kodu (Resimlerin otomatik değişmesini sağlar) -->
    <script>
        let slides = document.querySelectorAll('.slide');
        let currentSlide = 0;

        function nextSlide() {
            slides[currentSlide].classList.remove('active');
            currentSlide = (currentSlide + 1) % slides.length;
            slides[currentSlide].classList.add('active');
        }

        setInterval(nextSlide, 4000); // Her 4 saniyede bir resim değişir
    </script>

</body>
</html>
