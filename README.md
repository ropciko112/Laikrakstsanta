<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Source+Sans+Pro:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #2c5aa0;
            --secondary: #d4af37;
            --dark: #1a1a1a;
            --light: #f8f9fa;
            --accent: #e63946;
            --gray: #6c757d;
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Source Sans Pro', sans-serif;
            background-color: #f0f2f5;
            color: #333;
            line-height: 1.6;
        }

        /* Header Styles */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, #1e4088 100%);
            color: white;
            padding: 1.5rem 2rem;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: relative;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
        }

        .header-left {
            font-size: 0.9rem;
            opacity: 0.9;
        }

        .header-center h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin: 0;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
            text-align: center;
        }

        .header-right {
            background-color: rgba(255, 255, 255, 0.15);
            padding: 0.6rem 1rem;
            border-radius: 8px;
            text-align: center;
            backdrop-filter: blur(5px);
            min-width: 120px;
        }

        #current-date, #current-time {
            display: block;
            font-size: 0.9rem;
            font-weight: 600;
        }

        /* Navigation */
        nav {
            background-color: white;
            padding: 1rem;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }

        .nav-container {
            display: flex;
            justify-content: center;
            max-width: 1200px;
            margin: 0 auto;
        }

        nav a {
            color: var(--dark);
            margin: 0 1.2rem;
            text-decoration: none;
            font-weight: 600;
            text-transform: uppercase;
            font-size: 0.95rem;
            transition: var(--transition);
            position: relative;
            padding: 0.5rem 0;
        }

        nav a:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: var(--secondary);
            transition: var(--transition);
        }

        nav a:hover {
            color: var(--primary);
        }

        nav a:hover:after {
            width: 100%;
        }

        /* Main Content */
        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 1.5rem;
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
        }

        @media (min-width: 768px) {
            .container {
                grid-template-columns: 3fr 2fr;
            }
        }

        /* Card Styles */
        .card {
            background-color: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transition: var(--transition);
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.12);
        }

        .card-header {
            background: linear-gradient(135deg, var(--primary) 0%, #3a6cc0 100%);
            color: white;
            padding: 1.2rem 1.5rem;
            position: relative;
        }

        .card-header h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            margin: 0;
            display: flex;
            align-items: center;
        }

        .card-header h3 i {
            margin-right: 0.7rem;
            font-size: 1.3rem;
        }

        .card-body {
            padding: 1.5rem;
        }

        /* Audio Player */
        .audio-player {
            text-align: center;
            background: linear-gradient(to bottom, #f8f9fa, #e9ecef);
            border-left: 4px solid var(--secondary);
        }

        .audio-player h3 {
            color: var(--dark);
            margin-bottom: 1rem;
        }

        audio {
            width: 100%;
            margin-top: 0.5rem;
            border-radius: 30px;
        }

        /* Facts List */
        .facts-list {
            list-style: none;
        }

        .facts-list li {
            margin-bottom: 1.2rem;
            padding-left: 1.5rem;
            position: relative;
            border-left: 3px solid transparent;
            transition: var(--transition);
        }

        .facts-list li:hover {
            border-left-color: var(--secondary);
        }

        .facts-list li:before {
            content: "•";
            color: var(--secondary);
            font-weight: bold;
            display: inline-block;
            position: absolute;
            left: 0;
            font-size: 1.5rem;
            line-height: 1;
        }

        /* Weather Section */
        #weather {
            display: flex;
            align-items: center;
            font-size: 1.1rem;
        }

        #weather i {
            font-size: 2rem;
            color: var(--primary);
            margin-right: 1rem;
        }

        .weather-info {
            display: flex;
            flex-direction: column;
        }

        /* Joke Section */
        .joke-section {
            text-align: center;
        }

        .joke-section img {
            max-width: 100%;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }

        .joke-section img:hover {
            transform: scale(1.02);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.15);
        }

        /* Footer */
        footer {
            background: linear-gradient(135deg, var(--dark) 0%, #2c2c2c 100%);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 3rem;
            font-size: 0.9rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
                gap: 1rem;
            }
            
            .header-center h1 {
                font-size: 2rem;
            }
            
            .nav-container {
                flex-direction: column;
                align-items: center;
                gap: 0.5rem;
            }
            
            nav a {
                margin: 0.5rem 0;
            }
            
            .container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-content">
            <div class="header-left">Nr. 14</div>
            <div class="header-center">
                <h1>Laikraksts ANTA</h1>
            </div>
            <div class="header-right">
                <span id="current-date">Ielādē datumu...</span>
                <span id="current-time">Ielādē laiku...</span>
            </div>
        </div>
    </header>

    <nav>
        <div class="nav-container">
            <a href="docs/galerija.html"><i class="fas fa-images"></i> Galerija</a>
            <a href="docs/game.html"><i class="fas fa-gamepad"></i> Spēle</a>
        </div>
    </nav>

    <div class="container">
        <main class="main-content">
            <!-- Audio Player Section -->
            <div class="card audio-player">
                <div class="card-body">
                    <h3><i class="fas fa-music"></i> Klausies dziesmu "Antas piedzīvojumi"</h3>
                    <audio controls>
                        <source src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/main/docs/Antas%20piedz%C4%ABvojumi.mp3%20(1)" type="audio/mpeg">
                        Jūsu pārlūkprogramma neatbalsta audio atskaņošanu.
                    </audio>
                </div>
            </div>

            <!-- Vārda diena Section -->
            <div class="card">
                <div class="card-header">
                    <h3><i class="fas fa-birthday-cake"></i> Vārda diena</h3>
                </div>
                <div class="card-body">
                    <p>Šodien vārda dienas svin: <strong>Lolita, Vitolds</strong>.</p>
                </div>
            </div>

            <!-- Fakti Section -->
            <div class="card">
                <div class="card-header">
                    <h3><i class="fas fa-star"></i> Interesanti fakti par Antu</h3>
                </div>
                <div class="card-body">
                    <ul class="facts-list">
                        <li><strong>Antu un Juri IVP kopā sauc par saldo pārīti.</strong></li>
                        <li><strong>Antai patīk, kad viņu kāds cenšas ievērt durvīs.</strong></li>
                        <li><strong>Antas mīļākais ēdiens ir medus kūka.</strong></li>
                        <li><strong>Anta nāk uz darbu ātrāk, lai varētu paspēlēties ar sunīšu mantiņu.</strong></li>
                    </ul>
                </div>
            </div>
        </main>

        <aside class="sidebar">
            <!-- Laikapstākļi Section -->
            <div class="card">
                <div class="card-header">
                    <h3><i class="fas fa-cloud-sun"></i> Laikapstākļi Rīgā</h3>
                </div>
                <div class="card-body">
                    <div id="weather">
                        <i class="fas fa-cloud-sun-rain"></i>
                        <div class="weather-info">
                            <span id="weather-desc">Ielādē laikapstākļus...</span>
                            <span id="weather-temp"></span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Joks Section -->
            <div class="card joke-section">
                <div class="card-header">
                    <h3><i class="fas fa-smile"></i> Dienas Joks</h3>
                </div>
                <div class="card-body">
                    <img src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/20250416_1136_Kafija%20un%20burk%C4%81ni_remix_01jryvrwbte56s703aad3vx95k.png" alt="Dienas joks" />
                </div>
            </div>
        </aside>
    </div>

    <footer>
        <div class="footer-content">
            <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas.</p>
            <p>PS: Lapa ir domāta kā joks un nav jāuztver nopietni!</p>
        </div>
    </footer>

    <script>
        function updateTimeAndDate() {
            const now = new Date();
            const options = { day: 'numeric', month: 'long', year: 'numeric' };
            const timeOptions = { hour: '2-digit', minute: '2-digit', second: '2-digit' };
            
            document.getElementById('current-date').textContent = now.toLocaleDateString('lv-LV', options);
            document.getElementById('current-time').textContent = now.toLocaleTimeString('lv-LV', timeOptions);
        }

        function getWeather() {
            const weatherElement = document.getElementById('weather-desc');
            const tempElement = document.getElementById('weather-temp');
            const apiKey = "1b5e2264709b5eacd217f25ebf6dc09a";
            const city = "Riga";
            const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}&units=metric&lang=lv`;

            fetch(apiUrl)
                .then(response => response.json())
                .then(data => {
                    if (data.main) {
                        weatherElement.textContent = data.weather[0].description;
                        tempElement.textContent = `Temperatūra: ${Math.round(data.main.temp)}°C`;
                    } else {
                        weatherElement.textContent = "Nevarēja iegūt laikapstākļus.";
                    }
                })
                .catch(error => {
                    weatherElement.textContent = "Kļūda, mēģini vēlreiz.";
                    console.error("Error fetching weather data:", error);
                });
        }

        // Initialize functions
        setInterval(updateTimeAndDate, 1000);
        updateTimeAndDate();
        getWeather();
    </script>
</body>
</html>
