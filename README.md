<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой Сайт</title>
</head>
<body>
    
  
    <header>
        <h1>ПРИБОРНЫЙ ЗАВОД «СИГНАЛ»</h1>
    </header>
    

    <main>
        <div class="slider">
            <div class="slides">
                <div class="slide">
                    <h2>Технические средства САС СЦР</h2>
                    <img src="https://pz-signal.ru/storage/app/media/kollazh_1_1.jpg" alt="Продукт 1">
                    <p>Комплекс технических средств для организации САС СЦР на объектах использования атомной энергетики</p>
                    <button class="buy-button" onclick="window.location.href='https://www.pz-signal.ru/'">Купить</button>
                </div>
                <div class="slide">
                    <h2>Комплексная система контроля и защиты</h2>
                    <img src="https://pz-signal.ru/storage/app/uploads/public/607/d58/9eb/607d589ebdbac819999374.jpeg" alt="Продукт 2">
                    <p>Это высокотехнологичное решение для автоматизации процессов мониторинга объектов различного назначения.КСКУЗ обеспечивает безопасность,надежность работы систем на объектах.</p>
                    <button class="buy-button" onclick="window.location.href='https://www.pz-signal.ru/'">Купить</button>
                </div>
                <div class="slide">
                    <h2>Вставки кабельные</h2>
                    <img src="https://pz-signal.ru/storage/app/uploads/public/604/a37/7a6/604a377a68dcd102149243.jpg" alt="Продукт 3">
                    <p>Вхлдят в состав сервопривода РР, АР РБМ-К7.Сб.237 и предназначена для обеспечения электрической связи кабеля с устройствами сервопривода.</p>
                    <button class="buy-button" onclick="window.location.href='https://www.pz-signal.ru/'">Купить</button>
                </div>
                <div class="slide">
                    <h2>Стенд моделирования функциональных алгоритмов</h2>
                    <img src="https://pz-signal.ru/storage/app/uploads/public/618/e76/67b/618e7667bed3b096380039.jpg" alt="Продукт 4">
                    <p>Стенд моделирования функциональных алгоритмов КСКУЗ энергоблоков АЭС используется для изучения алгоритмов работы системы, моделирования аппаратных средств и дефектов, тестирования обновлений перед внедрением, а также для проверки действий персонала в различных ситуациях. </p>
                    <button class="buy-button" onclick="window.location.href='https://www.pz-signal.ru/'">Купить</button>
                </div>
                <div class="slide">
                    <h2>Микроцентрифуга "Сигмед"МЦ-1</h2>
                    <img src="https://pz-signal.ru/storage/app/uploads/public/620/13d/35c/62013d35c600d259166701.png" alt="Продукт 5">
                    <p>Предназначена для низкоскоростного центрифугирования жидкостей в пробирках, перемешивания жидкостей с помощью магнитной насадки.</p>
                    <button class="buy-button" onclick="window.location.href='https://www.pz-signal.ru/'">Купить</button>
                </div>
                <div class="slide">
                    <h2>Микроцентрифуга "Сигмед"МЦ-2</h2>
                    <img src="https://pz-signal.ru/storage/app/uploads/public/620/148/359/6201483598688826870140.png" alt="Продукт 6">
                    <p>Предназначена для разделения по плотностям под действием центробежных сил исследоваемых компонентов в пробирках, установленных в ротор</p>
                    <button class="buy-button" onclick="window.location.href='https://www.pz-signal.ru/'">Купить</button>
                </div>
            </div>
            <div class="navigation">
                <button class="nav-button" onclick="prevSlide()">&#10094;</button>
                <button class="nav-button" onclick="nextSlide()">&#10095;</button>
            </div>
        </div>
        <script>let currentSlide = 0;

            function showSlide(index) {
                const slides = document.querySelector('.slides');
                const totalSlides = document.querySelectorAll('.slide').length;
                if (index >= totalSlides) {
                    currentSlide = 0;
                } else if (index < 0) {
                    currentSlide = totalSlides - 1;
                } else {
                    currentSlide = index;
                }
                slides.style.transform = 'translateX(' + (-currentSlide * 100) + '%)';
            }
            
            function nextSlide() {
                showSlide(currentSlide + 1);
            }
            
            function prevSlide() {
                showSlide(currentSlide - 1);
            }</script>
            <style>body {
                font-family: Arial, sans-serif;
                background-color: #f4f4f4;
                margin: 0;
                padding: 0;
                display: flex;
                flex-direction: column; 
                height: 100vh; 
                justify-content: space-between; 
            }
            
            header {
                background-color: #2D2B8B;
                color: white;
                text-align: center;
                padding: 20px;
            }
            
            
            main {
                flex-grow: 1; 
                display: flex;
                justify-content: center; 
                align-items: center; 
            }
            
            
            .slider {
                width: 100%;
                max-width: 900px; 
                position: relative;
                overflow: hidden;
                border: 2px solid #ccc;
                border-radius: 10px;
                background: white;
            }
            
            
            .slides {
                display: flex;
                transition: transform 0.5s ease;
            }
            
            .slide {
                min-width: 100%; 
                box-sizing: border-box;
                text-align: center;
            }
            
            .slide img {
                max-width: 100%; 
                border-radius: 10px;
            }
            
            
            .slide h2 {
                color: #2D2B8B; 
                font-size: 24px;
                margin-bottom: 15px; 
            }
            
            
            .navigation {
                position: absolute;
                top: 50%;
                width: 100%;
                display: flex;
                justify-content: space-between;
                transform: translateY(-50%);
            }
            
            .nav-button {
                background-color: rgba(0, 0, 0, 0.5);
                color: white;
                border: none;
                padding: 30px;
                cursor: pointer;
                border-radius: 5px;
            }
            
            .nav-button:hover {
                background-color: rgba(0, 0, 0, 0.8);
            }
            
            
            .buy-button {
                background-color: #2D2B8B; 
                color: white;
                border: none;
                padding: 15px 30px; 
                font-size: 18px; 
                border-radius: 5px; 
                cursor: pointer;
                transition: background-color 0.3s ease;
                width: 100%; 
                max-width: 250px; 
                margin-top: 10px; 
            }
            
            .buy-button:hover {
                background-color: #1a1a7e; 
            }
            
            
            footer {
                background-color: #333;
                color: white;
                text-align: center;
                padding: 10px;
                width: 100%;
                box-sizing: border-box;
            }
            h1,h2 {
                font-family: 'Bebas Neue', sans-serif;
            }
            </style>
    </main>
    

    <footer>
        <p>&copy; 2024 ПАО Сигнал. Все права защищены.</p>
    </footer>

</body>
</html>
