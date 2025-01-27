<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <style>
        /* CSS Stili */
        body {
            font-family: "Georgia", "Times New Roman", serif;
            background-color: #a1832b;
            margin: 0;
            padding: 0;
            color: #333;
        }
        header {
            background-color: #2c2c2c;
            color: white;
            padding: 20px 40px;
            text-align: center;
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-family: 'Georgia', serif;
        }
        .header-left, .header-right {
            font-size: 14px;
        }
        h1 {
            font-size: 36px;
            margin: 0;
            font-family: 'Georgia', serif;
        }
        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 20px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
        }
        nav a:hover {
            color: #ddd;
        }
        .section {
            padding: 30px;
            background-color: white;
            margin: 20px auto;
            border-radius: 10px;
            width: 80%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
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
        /* Laikapstākļu sadaļa - caurspīdīgums */
        #weather {
            background-color: rgba(240, 240, 240, 0.8); /* Caurspīdīgs gaišais fons */
            padding: 15px;
            border-radius: 5px;
            font-size: 18px;
            font-family: 'Georgia', serif;
            border: 1px solid #ccc;
        }

footer {
    background-color: #2c2c2c;
    color: white;
    text-align: center;
    padding: 15px;
    font-family: 'Georgia', serif;
    position: sticky;
    bottom: 0;
    width: 100%;
    z-index: 1000; /* Nodrošina, ka tas paliek virs citiem elementiem */
}

footer p {
    margin: 0;
    font-size: 18px;
}
        .footer-joke-text {
            font-size: 18px;
            font-family: 'Georgia', serif;
            margin-top: 10px;
        }
        .footer-image {
            display: block;
            margin: 10px auto;
            max-width: 100%;
            height: auto;
            border: 2px solid #ccc;
        }
        /* Dienas joks sadaļai */
        .jokes-section {
            padding: 30px;
            background-color: #ffffff;
            margin: 20px auto;
            border-radius: 10px;
            width: 80%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        .jokes-section img {
            max-width: 100%;
            border-radius: 10px;
        }
        /* Centrēts teksts footer */
        .footer-text-center {
            text-align: center;
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 11</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">
            <span id="current-date">Ielādē datumu...</span><br>
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
            <p><strong>Ziloņi ir vienīgie dzīvnieki, kas nevar lēkt</strong><br />To masīvais ķermenis un īpa&scaron;ā kāju uzbūve to padara fiziski neiespējamu.</p>
<li>
<p><strong>Panda mazuļi dzimst sīki &ndash; vēl mazāki nekā pele</strong><br />Lielākie panda mazuļi sver tikai apmēram 100 gramus, bet pieaugu&scaron;ie var sverēt līdz 150 kg.</p>
</li>
<li>
<p><strong>Zirņu gliemeži var gulēt līdz 3 gadiem</strong><br />Ja apstākļi nav labvēlīgi, tie spēj iemiglot uz ilgu laiku, līdz atkal ir piemērota vide.</p>
</li>
<li>
<p><strong>Austrālijas krokodili spēj peldēt ar ātrumu līdz 29 km/h</strong><br />Tie ir vieni no ātrākajiem reptīļiem ūdenī.</p>
</li>
<li>
<p><strong>Govs var uzkāpt aug&scaron;up pa kāpnēm, bet nevar nokāpt lejā</strong><br />To kāju uzbūve un lielais ķermenis to padara gandrīz neiespējamu.</p>
</li>
<li>
<p><strong>Delfīni spēj atpazīt sevi spogulī</strong><br />Tie ir vieni no nedaudzajiem dzīvniekiem, kas demonstrē pa&scaron;apziņu.</p>
</li>
<li>
<p><strong>Ķirzakas spēj atjaunot savu asti, ja tā ir zaudēta</strong><br />&Scaron;ī spēja saucas regenerācija, un tā ir viens no interesantākajiem dzīvnieku valsts fenomeniem.</p>
</li>
<li>
<p><strong>Karūsu zivis ir vienīgie dzīvnieki, kas spēj pārvērsties no mātītes uz tēviņu</strong><br />Tas notiek, ja grupā nav pietiekami daudz tēviņu.</p>
</li>
<li>
<p><strong>Sienāži spēj gulēt ar vienu atvērtu aci</strong><br />Tas ļauj viņiem būt modriem un uzmanīgiem pret plēsējiem, pat atpū&scaron;oties.</p>
</li>
<li>
<p><strong>Kāpuru sirds atrodas to galvā</strong><br />&Scaron;ie vēžveidīgie ir unikāli ar to, ka to sirds, smadzenes un citi orgāni atrodas galvas daļā.</p>
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
