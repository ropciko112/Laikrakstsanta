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
            background: linear-gradient(to bottom, #f0f2f5, #e6e9f0);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }

        /* Header Styles */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, #1e4088 100%);
            color: white;
            padding: 1.2rem 2rem;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .header-left {
            font-size: 0.9rem;
            opacity: 0.9;
        }

        .header-center h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.2rem;
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
            padding: 0.8rem;
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
        .main-container {
            max-width: 1200px;
            width: 100%;
            margin: 1.5rem auto;
            padding: 0 1.5rem;
            flex: 1;
        }

        .content-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        @media (min-width: 992px) {
            .content-grid {
                grid-template-columns: 2fr 1fr;
            }
        }

        /* Card Styles */
        .card {
            background-color: white;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transition: var(--transition);
            height: fit-content;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.12);
        }

        .card-header {
            background: linear-gradient(135deg, var(--primary) 0%, #3a6cc0 100%);
            color: white;
            padding: 1rem 1.5rem;
            position: relative;
        }

        .card-header h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.4rem;
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
            grid-column: 1 / -1;
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
            padding: 0.5rem 0 0.5rem 1.5rem;
        }

        .facts-list li:hover {
            border-left-color: var(--secondary);
            background-color: #f9f9f9;
            padding-left: 1.8rem;
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
            padding: 1rem 0;
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

        /* Main content sections */
        .main-content {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .sidebar {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        /* Footer */
        footer {
            background: linear-gradient(135deg, var(--dark) 0%, #2c2c2c 100%);
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 2rem;
            font-size: 0.9rem;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: var(--transition);
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.1);
        }

        .social-links a:hover {
            transform: translateY(-3px);
            background-color: rgba(255, 255, 255, 0.2);
        }

        .social-links .fa-facebook:hover {
            color: #3b5998;
        }

        .social-links .fa-linkedin:hover {
            color: #0077b5;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
                gap: 0.8rem;
                padding: 1rem;
            }
            
            .header-center h1 {
                font-size: 1.8rem;
            }
            
            .nav-container {
                flex-direction: column;
                align-items: center;
                gap: 0.5rem;
            }
            
            nav a {
                margin: 0.3rem 0;
            }
            
            .content-grid {
                grid-template-columns: 1fr;
            }
            
            .audio-player {
                grid-column: 1;
            }
            
            .social-links {
                flex-wrap: wrap;
                gap: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left"></div>
        <div class="header-center">
            <h1>Laikraksts ANTA</h1>
        </div>
        <div class="header-right">
            <span id="current-date">Ielādē datumu...</span>
            <span id="current-time">Ielādē laiku...</span>
        </div>
    </header>

    <nav>
        <div class="nav-container">
            <a href="docs/galerija.html"><i class="fas fa-images"></i> Galerija</a>
            <a href="docs/game.html"><i class="fas fa-gamepad"></i> Spēle</a>
        </div>
    </nav>

    <div class="main-container">
        <div class="content-grid">
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

            <div class="main-content">
                <!-- Vārda diena Section -->
                <div class="card">
                    <div class="card-header">
                        <h3><i class="?"></i> Ticējumi par Antu</h3>
                    </div>
                    <div class="card-body">
                        <ul class="facts-list">
                            <li><strong>Ja Anta ieiet virtuvē un nopūšas, tad ledusskapī pašā no sevis pazūd siers.</strong></li>
                            <li><strong>Ja Anta pasaka “ātri būšu atpakaļ”, tad zini – viņa atgriezīsies tikai tad, kad mēness būs nomainījis fāzi.</strong></li>
                            <li><strong>Ja Anta apsēžas uz dīvāna “tikai uz minūti”, tad televizora pults noslēpumaini pazūd.</strong></li>
                            <li><strong>Ja Anta nolemj “neēst saldumus”, tad veikalā tieši tajā dienā ir atlaides uz šokolādi.</strong></li>
                            <li><strong>Ja Anta paskatās uz pulksteni un saka: “Ak, vēl daudz laika!”, tad noteikti jau ir par vēlu..</strong></li>
                            <li><strong>Ja Anta piezvana, tad telefons kā minimums 2 reizes nogāžas no galda pats no sevis.</strong></li>
                            <li><strong>Ja Anta saka “Es uz īsu brīdi”, tad tad kā minimums uz 1H.</strong></li>
                            <li><strong>Ja Anta iesmejas, tad tuvākās 3 mājas suņi momentā pamostas un sāk prasīt ēst.</strong></li>
                        </ul>
                    </div>
                    <div class="card-body">
                        <p> <strong>  </strong>.</p>
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
            </div>

            <div class="sidebar">
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
            </div>
        </div>
    </div>

    <footer>
        <div class="footer-content">
            <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas.</p>
            <p>PS: Lapa ir domāta kā joks un nav jāuztver nopietni!</p>
            
            <div class="social-links">
                <a href="https://www.facebook.com/anta.verdina" target="_blank" title="Facebook">
                    <i class="fab fa-facebook-f"></i>
                </a>
                <a href="https://www.linkedin.com/in/anta-klepecka-ex-v%C4%93rdi%C5%86a-12b29459/overlay/about-this-profile/" target="_blank" title="LinkedIn">
                    <i class="fab fa-linkedin-in"></i>
                </a>
            </div>
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
                        
                        // Update weather icon based on conditions
                        const weatherIcon = document.querySelector('#weather i');
                        if (data.weather[0].main === 'Clear') {
                            weatherIcon.className = 'fas fa-sun';
                        } else if (data.weather[0].main === 'Clouds') {
                            weatherIcon.className = 'fas fa-cloud';
                        } else if (data.weather[0].main === 'Rain') {
                            weatherIcon.className = 'fas fa-cloud-rain';
                        } else if (data.weather[0].main === 'Snow') {
                            weatherIcon.className = 'fas fa-snowflake';
                        }
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
