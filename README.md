# QazaqAl-5
Қазақ тілін оқытуға арналған ЖИ көмекші
<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QazaqAI 5 - 5-сынып Қазақ тілі</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary: #4F46E5;
            --secondary: #06B6D4;
            --accent: #F59E0B;
            --dark: #0F172A;
            --light: #F8FAFC;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            background-color: var(--light);
            color: #334155;
        }

        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            padding: 1.5rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .hero {
            background: linear-gradient(rgba(15, 23, 42, 0.8), rgba(15, 23, 42, 0.8)), 
                        url('https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=1200&q=80') center/cover;
            color: white;
            text-align: center;
            padding: 4rem 1rem;
        }

        .hero h1 { font-size: 2.5rem; margin-bottom: 0.5rem; }
        .hero p { font-size: 1.2rem; opacity: 0.9; }

        .container {
            max-width: 1100px;
            margin: 2rem auto;
            padding: 0 1rem;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 2rem;
            color: var(--dark);
        }

        .card-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .card {
            background: white;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.12);
        }

        .card-img {
            height: 180px;
            width: 100%;
            object-fit: cover;
        }

        .card-body {
            padding: 1.5rem;
        }

        .tag {
            display: inline-block;
            background: #EEF2FF;
            color: var(--primary);
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 10px;
        }

        .btn {
            display: inline-block;
            width: 100%;
            padding: 10px;
            background: var(--primary);
            color: white;
            text-align: center;
            border-radius: 8px;
            border: none;
            cursor: pointer;
            font-weight: 600;
            margin-top: 10px;
            transition: 0.2s;
        }

        .btn:hover { background: #4338CA; }

        /* AI Chat Widget */
        .ai-chat-box {
            background: white;
            border-radius: 16px;
            padding: 1.5rem;
            margin-top: 3rem;
            box-shadow: 0 10px 25px rgba(0,0,0,0.05);
            border: 2px solid #E0E7FF;
        }

        .chat-history {
            height: 150px;
            background: #F8FAFC;
            border-radius: 8px;
            padding: 1rem;
            margin-bottom: 1rem;
            overflow-y: auto;
        }

        .chat-input {
            display: flex;
            gap: 10px;
        }

        .chat-input input {
            flex: 1;
            padding: 12px;
            border: 1px solid #CBD5E1;
            border-radius: 8px;
            outline: none;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo"><i class="fa-solid fa-brain"></i> QazaqAI 5</div>
        <div>5-сынып Қазақ тілі порталы</div>
    </header>

    <section class="hero">
        <h1>Қазақ тілін ЖИ көмегімен меңгер!</h1>
        <p>Бейнесабақтар, аудиотапсырмалар және AI-ассистент көмегімен біліміңді шыңда</p>
    </section>

    <div class="container">
        <h2 class="section-title">📚 Оқу модульдері</h2>

        <div class="card-grid">
            <!-- 1-Тақырып: Бейнесабақ -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1577896851231-70ef18881754?auto=format&fit=crop&w=600&q=80" class="card-img" alt="Бейнесабақ">
                <div class="card-body">
                    <span class="tag"><i class="fa-solid fa-play"></i> Бейнесабақ</span>
                    <h3>1. Зат есімнің септелуі</h3>
                    <p>Септік жалғауларының ережелерін видео арқылы көрнекі түрде меңгеріңіз.</p>
                    <button class="btn"><i class="fa-solid fa-circle-play"></i> Видеоны қарау</button>
                </div>
            </div>

            <!-- 2-Тақырып: Аудиотапсырма -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1590602847861-f357a9332bbc?auto=format&fit=crop&w=600&q=80" class="card-img" alt="Аудиотапсырма">
                <div class="card-body">
                    <span class="tag" style="color:#059669; background:#ECFDF5;"><i class="fa-solid fa-headphones"></i> Аудиотапсырма</span>
                    <h3>2. Мәтінді тыңдап, түсіну</h3>
                    <p>Мәтінді мұқият тыңдап, басты ойды анықтауға арналған жаттығу.</p>
                    <button class="btn" style="background:#059669;"><i class="fa-solid fa-volume-high"></i> Аудионы тыңдау</button>
                </div>
            </div>

            <!-- 3-Тақырып: Онлайн Тест -->
            <div class="card">
                <img src="https://images.unsplash.com/photo-1606326608606-aa0b62935f2b?auto=format&fit=crop&w=600&q=80" class="card-img" alt="Тест">
                <div class="card-body">
                    <span class="tag" style="color:#D97706; background:#FEF3C7;"><i class="fa-solid fa-pen-to-square"></i> Онлайн Тест</span>
                    <h3>3. Бекіту сұрақтары</h3>
                    <p>Өткен тақырыптар бойынша біліміңді тексеріп, бал жина!</p>
                    <button class="btn" style="background:#D97706;"><i class="fa-solid fa-check-double"></i> Тестті бастау</button>
                </div>
            </div>
        </div>

        <!-- ЖИ Ассистент бөлімі -->
        <div class="ai-chat-box">
            <h3><i class="fa-solid fa-robot" style="color: var(--primary);"></i> QazaqAI Көмекшісі (ЖИ-мен сұрақ-жауап)</h3>
            <p style="font-size: 0.9rem; color: #64748B;">Қазақ тілі ережелері немесе тапсырмалар бойынша сұрағыңды қой:</p>
            <div class="chat-history">
                <p><strong>AI:</strong> Сәлем! Мен QazaqAI көмекшісімін. 5-сынып қазақ тілі сабағынан қандай сұрағың бар?</p>
            </div>
            <div class="chat-input">
                <input type="text" placeholder="Мұнда сұрағыңды жаз (мысалы: Зат есім деген не?)...">
                <button class="btn" style="width: auto; padding: 0 20px;"><i class="fa-solid fa-paper-plane"></i> Жіберу</button>
            </div>
        </div>
    </div>

</body>
</html>
