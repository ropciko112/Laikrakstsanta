<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <style>
        /* Pamata stili */
        body {
            font-family: "Georgia", "Times New Roman", serif;
            background-color: #a1832b;
            margin: 0;
            padding: 0;
            color: #333;
        }

        /* Galvene */
        header {
            background: linear-gradient(135deg, #2c2c2c, #1a1a1a);
            color: white;
            padding: 20px 40px;
            text-align: center;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .header-left {
            font-size: 14px;
        }

        .header-right {
            font-size: 16px;
            text-align: right;
            background-color: rgba(255, 255, 255, 0.1); /* Caurspīdīgs fons */
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        h1 {
            font-size: 36px;
            margin: 0;
            font-family: 'Georgia', serif;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        #current-date, #current-time {
            display: block;
            font-size: 16px;
            font-weight: bold;
            color: white;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        /* Navigācija */
        nav {
            background-color: #444;
            padding: 15px;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        nav a {
            color: white;
            margin: 0 20px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 16px;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        nav a:hover {
            color: #ddd;
            transform: translateY(-2px);
        }

        /* Sekcijas */
        .section {
            padding: 30px;
            background-color: white;
            margin: 20px auto;
            border-radius: 12px;
            width: 80%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        h3 {
            font-size: 24px;
            font-weight: bold;
            text-transform: uppercase;
            color: #2c2c2c;
            margin-bottom: 15px;
        }

        p, li {
            font-size: 18px;
            line-height: 1.6;
        }

        ul.facts-list {
            list-style-type: none;
            padding-left: 0;
        }

        ul.facts-list li {
            margin-bottom: 20px;
        }

        /* Laikapstākļu sadaļa */
        #weather {
            background-color: rgba(240, 240, 240, 0.8);
            padding: 15px;
            border-radius: 8px;
            font-size: 18px;
            font-family: 'Georgia', serif;
            border: 1px solid #ccc;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        /* Kājene */
        footer {
            background: linear-gradient(135deg, #2c2c2c, #1a1a1a);
            color: white;
            text-align: center;
            padding: 20px;
            font-family: 'Georgia', serif;
            position: sticky;
            bottom: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.2);
        }

        footer p {
            margin: 0;
            font-size: 18px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        /* Dienas joks sadaļa */
        .jokes-section {
            padding: 30px;
            background-color: #ffffff;
            margin: 20px auto;
            border-radius: 12px;
            width: 80%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .jokes-section img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 11</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">
            <span id="current-date">Ielādē datumu...</span>
            <span id="current-time">Ielādē laiku...</span>
        </div>
    </header>
    <nav>
        <a href="docs/galerija.html">Galerija</a>
        <a href="docs/game.html">Spēle</a>
    </nav>
    <!-- Vārda diena -->
    <div id="vardadiena" class="section">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienas svin: Kārlis, Spodris.</p>
    </div>
    <!-- Interesanti fakti -->
    <div id="fakti" class="section">
        <h3>Interesanti fakti par: Dzīvniekiem.</h3>
        <ul class="facts-list">
           <li>
<p><strong>Sirds sāk darboties jau pirms dzim&scaron;anas</strong><br />Cilvēka sirds sāk sisties apmēram 4 nedēļas pēc ieņem&scaron;anas, un tā turpina darboties visu mūžu.</p>
</li>
<li>
<p><strong>Sirds ikdienā saspiežas apmēram 100 000 reizes</strong><br />Tas nozīmē, ka vidēji mūža laikā sirds saspiežas vairāk nekā 2,5 miljardus reižu.</p>
</li>
<li>
<p><strong>Asinsvadi cilvēka ķermenī, ja tos savienotu vienā garā līnijā, varētu aptvert Zemi 2,5 reizes</strong><br />Kopējais asinsvadu garums ir apmēram 100 000 kilometru.</p>
</li>
<li>
<p><strong>Sirds izspiež apmēram 70 ml asins ar katru sitienu</strong><br />Tas nozīmē, ka vienā minūtē sirds izspiež apmēram 5 litrus asins.</p>
</li>
<li>
<p><strong>Asinis veic pilnu apgriezienu ķermenī apmēram 20 sekunžu laikā</strong><br />Tas nozīmē, ka asinis pārvietojas ar ātrumu aptuveni 2 km/h.</p>
</li>
<li>
<p><strong>Sirds ir vienīgais orgāns, kas spēj darboties neatkarīgi no smadzenēm</strong><br />Tam ir savs elektriskais sistēma, kas kontrolē tā darbību.</p>
</li>
<li>
<p><strong>Asins sastāvā ir 55% plazma un 45% asins &scaron;ūnas</strong><br />Plazma galvenokārt sastāv no ūdens, bet asins &scaron;ūnas ietver sarkanos un baltos asinsķermenī&scaron;us, kā arī trombocītus.</p>
</li>
<li>
<p><strong>Sirds svarā ir tikai apmēram 300 grami</strong><br />Neskatoties uz mazo svaru, tā ir viena no visspēcīgākajām muskuļu grupām cilvēka ķermenī.</p>
</li>
<li>
<p><strong>Asinsgrupu sistēmu atklāja 1901. gadā</strong><br />Austrie&scaron;u ārsts Kārlis Land&scaron;teiners atklāja, ka cilvēkiem ir dažādas asins grupas, kas ir būtiski asins pārlie&scaron;anas procedūrām.</p>
</li>
<li>
<p><strong>Sirds var turpināt sisties pat ārpus ķermeņa</strong><br />Ja sirdij ir piegādāts pietiekams daudzums skābekļa, tā var turpināt darboties pat tad, ja tā ir izņemta no ķermeņa.</p>
</li>
        </ul>
    </div>
    <!-- Laikapstākļi -->
    <div id="laikapstakli" class="section">
        <h3>Laikapstākļi Rīgā</h3>
        <div id="weather">Ielādē laikapstākļus...</div>
    </div>
    <!-- Dienas Joks -->
    <div id="joks" class="jokes-section">
        <h3>Dienas Joks</h3>
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/9i5bnr.jpg" />
    </div>
    <footer>
        <p class="footer-text-center">&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. PS: Lapa ir domāta kā joks un nav jāuztver nopietni!</p>
    </footer>
    <script>
        // Funkcija, lai parādītu pašreizējo laiku un datumu
        function updateTimeAndDate() {
            const now = new Date();
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            const day = String(now.getDate()).padStart(2, '0');
            const month = String(now.getMonth() + 1).padStart(2, '0');
            const year = now.getFullYear();
            const timeString = `${hours}:${minutes}:${seconds}`;
            const dateString = `${day}.${month}.${year}`;
            document.getElementById('current-time').textContent = timeString;
            document.getElementById('current-date').textContent = dateString;
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

        // Atjaunot laiku un datumu katru sekundi
        setInterval(updateTimeAndDate, 1000);

        // Iegūt laikapstākļus uzreiz
        getWeather();
    </script>
</body>
</html>
