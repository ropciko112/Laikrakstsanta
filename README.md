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
            position: fixed;
            width: 100%;
            bottom: 0;
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
        <div class="header-left">Nr. 7</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">
            <span id="current-date">Ielādē datumu...</span><br>
            <span id="current-time">Ielādē laiku...</span>
        </div>
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
        <p>Šodien vārda dienas svin Austris.</p>
    </div>

    <!-- Interesanti fakti -->
    <div id="fakti" class="section">
        <h3>Interesanti fakti par kosmosu</h3>
        <ul class="facts-list">
           <p><strong>Vārda izcelsme</strong>: Vārds "Anta" ir populārs vairākās valstīs, un tam var būt dažādas izcelsmes atkarībā no valsts vai kultūras. Latvie&scaron;u valodā "Anta" ir sievietes vārds, kas bieži tiek saistīts ar latviskiem un igauņu vārdiem, kas cēlu&scaron;ies no senām tradīcijām.</p>
<li>
<p><strong>Nezvaigžņu dzim&scaron;ana</strong> &ndash; Jauns zvaigznes veidojas galaktiku miglājos, kur gāzes un putekļi saspiežas un uzsilst, līdz sāk notikt kodolreakcijas, radot spožas zvaigznes.</p>
</li>
<li>
<p><strong>Kosmiskā vakuuma ietekme</strong> &ndash; Kosmosā ir ļoti maz vielas un atmosfēras, kas nozīmē, ka vakuuma stāvoklis ir ļoti tuvs, tāpēc skaņa nevar ceļot, jo nav pietiekami daudz molekulu, kas varētu pārnest vibrācijas.</p>
</li>
<li>
<p><strong>Melnie caurumi</strong> &ndash; Melnie caurumi ir kosmiskie objekti ar tādu masu un blīvumu, ka pat gaisma nevar izbēgt no to gravitācijas spēka. Tās ir radītas, sabrūkot masīvām zvaigznēm.</p>
</li>
<li>
<p><strong>Saules sistēma ir tikai maza daļa</strong> &ndash; Saules sistēma ir tikai neliela daļa no mūsu galaktikas "Piena Ceļa", kas ietver vairāk nekā 100 miljardia zvaigznes.</p>
</li>
<li>
<p><strong>Saules iznīcinā&scaron;ana</strong> &ndash; Pēc aptuveni 5 miljardiem gadu Saules kodolā izbeigsies ūdeņraža krājumi, un tā kļūs par sarkano milzi, kas iznīcinās Zemi.</p>
</li>
<li>
<p><strong>Kosmiskais atbalss</strong> &ndash; Pasaules radī&scaron;anas liecinieki &ndash; "kosmiskais mikrovīzijas fons" &ndash; ir radies no liela sprādziena, kas notika pirms aptuveni 13,8 miljardiem gadiem.</p>
</li>
<li>
<p><strong>Planētu dzīvotspēja</strong> &ndash; Lai uz planētas pastāvētu dzīvība, ir nepiecie&scaron;ams noteikts temperatūras diapazons, ūdens un atmosfēra, kas ir veicinājusi "Zemes" statusu kā vienīgo planētu, uz kuras zināms dzīvība pastāv.</p>
</li>
<li>
<p><strong>Tum&scaron;ā matērija un tum&scaron;ā enerģija</strong> &ndash; Lielākā daļa no visuma sastāv no tum&scaron;ās matērijas un tum&scaron;ās enerģijas, par kurām mēs joprojām īsti neko nezinām, bet tās ir galvenais spēks, kas nosaka galaktiku kustību un izple&scaron;anos.</p>
</li>
<li>
<p><strong>Kosmiskās sēklas</strong> &ndash; Zemes dzīvība var būt "izdzīvojusi" no kosmiskajiem sēklu mikroskopiskajiem organismiem, kas iespējams nonāku&scaron;i uz mūsu planētas, pārsprāgstot uz asteroīdiem.</p>
</li>
<li>
<p><strong>Bezgalīgais kosmoss</strong> &ndash; Kosmoss izskatās bezgalīgs, un pat mūsdienās zinātnieki vēl tikai sāk apzināt visuma apmērus. Tas varētu būt daudz lielāks, nekā mēs varam iedomāties.</p></li>
            <!-- Pievienojiet citus faktus -->
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
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/Angry%20Girl%20Meme.gif" />
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
