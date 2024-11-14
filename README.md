<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="mobile-web-app-capable" content="yes"> 
    <meta name="theme-color" content="#2D2B8B"> 
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <title>Мой Сайт</title>
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #f4f4f4;
        }
        
        header {
            background-color: #2D2B8B;
            color: white;
            padding: 15px;
        }
        
        .slider {
            border: 2px solid #ccc;
            border-radius: 10px;
            background: white;
        }
        
        .slide h2 {
            color: #2D2B8B;
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        .buy-button {
            background-color: #2D2B8B;
            color: white;
            font-size: 18px;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .buy-button:hover {
            background-color: #1a1a7e;
        }
        
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
        }
        
        h1, h2 {
            font-family: 'Bebas Neue', sans-serif;
        }
    </style>
</head>
<body>

    <header class="text-center">
        <h1>ПРИБОРНЫЙ ЗАВОД «СИГНАЛ»</h1>
    </header>

    <main class="container my-4">
        <div id="productCarousel" class="carousel slide slider mx-auto" data-bs-ride="carousel">
            <div class="carousel-inner">
                <div class="carousel-item active text-center p-4">
                    <h2>Технические средства САС СЦР</h2>
                    <img src="https://pz-signal.ru/storage/app/media/kollazh_1_1.jpg" class="d-block w-100 rounded" alt="Продукт 1">
                    <p class="mt-3">Комплекс технических средств для организации САС СЦР на объектах использования атомной энергетики</p>
                    <a href="https://www.pz-signal.ru/" class="btn buy-button mt-2">Купить</a>
                </div>
                <div class="carousel-item text-center p-4">
                    <h2>Комплексная система контроля и защиты</h2>
                    <img src="https://pz-signal.ru/storage/app/uploads/public/607/d58/9eb/607d589ebdbac819999374.jpeg" class="d-block w-100 rounded" alt="Продукт 2">
                    <p class="mt-3">Это высокотехнологичное решение для автоматизации процессов мониторинга объектов различного назначения. КСКУЗ обеспечивает безопасность, надежность работы систем на объектах.</p>
                    <a href="https://www.pz-signal.ru/" class="btn buy-button mt-2">Купить</a>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#productCarousel" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Предыдущий</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#productCarousel" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Следующий</span>
            </button>
        </div>
    </main>

    <footer>
        <p>&copy; 2024 ПАО Сигнал. Все права защищены.</p>
    </footer>

    <!-- Bootstrap JS and dependencies -->
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.min.js"></script>

</body>
</html>
