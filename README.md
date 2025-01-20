<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <style>
        /* CSS Stili */
        body {
            font-family: "Arial", sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 20px;
            text-align: center;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .header-left, .header-right {
            font-size: 14px;
        }

        h1 {
            font-size: 24px;
            margin: 0;
        }

        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }

        nav a:hover {
            color: #ccc;
        }

        .section {
            padding: 20px;
            background-color: white;
            margin: 10px;
            border-radius: 8px;
        }

        .facts-list {
            list-style-type: none;
            padding-left: 0;
        }

        .facts-list li {
            margin-bottom: 10px;
        }

        #weather {
            background-color: #ddd;
            padding: 10px;
            border-radius: 5px;
            font-size: 16px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
        }

        .footer-joke-text {
            font-size: 18px;
            text-align: center;
        }

        .footer-image {
            display: block;
            margin: 10px auto;
            max-width: 100%;
            height: auto;
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 5</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right"><span id="current-time">Ielādē laiku...</span></div>
    </header>
    
    <nav>
        <a href="#vardadiena">Vārda diena</a>
        <a href="#fakti">Interesanti fakti</a>
        <a href="#laikapstakli">Laikapstākļi</a>
        <a href="#joks">Dienas Joks</a>
    </nav>

    <!-- Vārda diena -->
    <div id="vardadiena" class="section">
        <h3>Vārda diena</h3>
        <p>&Scaron;odien vārda dienu svin: Agnese, Agnija, Agne.</p>
    </div>

    <!-- Interesanti fakti -->
    <div id="fakti" class="section">
        <h3>Interesanti fakti par grāmatvedību</h3>
        <ul class="facts-list">
            <li>
                <p><strong>Vārda izcelsme</strong>: Vārds "Anta" ir populārs vairākās valstīs, un tam var būt dažādas izcelsmes atkarībā no valsts vai kultūras. Latvie&scaron;u valodā "Anta" ir sievietes vārds, kas bieži tiek saistīts ar latviskiem un igauņu vārdiem, kas cēlu&scaron;ies no senām tradīcijām.</p>
            </li>
            <li>
                <p><strong>Vārda nozīme</strong>: Vārds "Anta" bieži tiek saistīts ar spēku un dzīvotspēju. Dažās interpretācijās tas var būt arī saistīts ar dabu, īpa&scaron;i augiem, un dzīvotspējīgām īpa&scaron;ībām.</p>
            </li>
        </ul>
    </div>

    <!-- Laikapstākļi -->
    <div id="laikapstakli" class="section">
        <h3>Laikapstākļi Rīgā</h3>
        <div id="weather">Ielādē laikapstākļus...</div>
    </div>

    <!-- Dienas Joks -->
    <div id="joks">
        <div class="footer-joke-text">Dienas Joks</div>
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/9hbp2q.jpg" alt="u/Low-Sir-7440 - vins" />
    </div>

    <footer>
        <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. PS: Lapa ir domāts kā joks un nav jāuztver nopietni!</p>
    </footer>

    <script>
        // Funkcija, lai parādītu pašreizējo laiku
        function updateTime() {
            const now = new Date();
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            const timeString = `${hours}:${minutes}:${seconds}`;
            document.getElementById('current-time').textContent = timeString;
        }

        // Iegūt laikapstākļus no API
        function getWeather() {
            const weatherElement = document.getElementById('weather');
            const apiKey = "1b5e2264709b5eacd217f25ebf6dc09a"; // Tava API atslēga
            const city = "Riga";
            const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}&units=metric&lang=lv`;

            fetch(apiUrl)
                .then(response => response.json())
                .then(data => {
                    if (data.main) {
                        weatherElement.textContent = `Šodien Rīgā: ${data.weather[0].description}, ${data.main.temp}°C`;
                    } else {
                        weatherElement.textContent = "Nevarēja iegūt laikapstākļus.";
                    }
                })
                .catch(error => {
                    weatherElement.textContent = "Kļūda, mēģini vēlreiz.";
                    console.error("Error fetching weather data:", error);
                });
        }

        // Atjaunot laiku katru sekundi
        setInterval(updateTime, 1000);

        // Iegūt laikapstākļus uzreiz
        getWeather();
    </script>
</body>
</html>
