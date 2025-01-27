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
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100%;
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
        <div class="header-left">Nr. 10</div>
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
        <a href="docs/galerija.html" target="_blank">Galerija</a>
    </nav>

    <!-- Vārda diena -->
    <div id="vardadiena" class="section">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienas svin: Ilze, Ildze, Izolde.</p>
    </div>

    <!-- Interesanti fakti -->
    <div id="fakti" class="section">
        <h3>Interesanti fakti par: Septiņiem pasaules brīnumiem.</h3>
        <ul class="facts-list">
            <p><strong>Pirmie brīnumi</strong>: Septiņi pasaules brīnumi sākotnēji tika uzskaitīti sengrieķu ceļotāju un vēsturnieku sarakstos, kas veidoti ap 200. gadu p.m.ē.</p>
            <li>
                <p><strong>Lielā piramīda</strong>: Lielā piramīda Gīzā (Ēģiptē) ir vienīgais no oriģinālajiem brīnumiem, kas saglabājies līdz mūsdienām.</p>
            </li>
            <li>
                <p><strong>Efesa Artemīdes templis</strong>: Šis templis, kas bija viens no pasaules brīnumiem, tika pilnībā iznīcināts 401. gadā mūsdienu Turcijā, kad to nodedzināja.</p>
            </li>
            <li>
                <p><strong>Maja kultūra</strong>: Pasaules brīnumos ir iekļauti arī uzlabotie Maja civilizācijas arhitektūras veidojumi, piemēram, Chichen Itza piramīda, kas atrodas Meksikā.</p>
            </li>
            <li>
                <p><strong>Hālīkarnassas mauzolejs</strong>: Šis monumentālais piemineklis, kas tika uzcelts Hālīkarnasā (mūsdienu Bodrumā, Turcija) ķēniša Mausolosa piemiņai, tika iznīcināts zemestrīces laikā 1300. gadā.</p>
            </li>
            <li>
                <p><strong>Koloss no Rodas</strong>: Šī milzīgā statuja stāvēja pie Rodes ostas un tika sabrukusi pēc zemestrīces 226. gadā p.m.ē.</p>
            </li>
            <li>
                <p><strong>Jūdas jūras pakājē</strong>: Pasaules brīnumi iekļāva arī Šaķara ezeru un tempļus, kas bija izcils piemērs romiešu impērijas arhitektūrai.</p>
            </li>
            <li>
                <p><strong>Mūsdienu brīnumi</strong>: 2007. gadā tika apstiprināti jauni septiņi pasaules brīnumi, tostarp Tadžmahal, Lielais Mura siena un Machu Picchu.</p>
            </li>
            <li>
                <p><strong>Maiju kalendārs un arhitektūra</strong>: Chichen Itza, viena no mūsdienu pasaules brīnumiem, ir pazīstama ar savu Maiju kalendāru, kas precīzi paredzēja solsticiju un citas astronomiskās parādības.</p>
            </li>
            <li>
                <p><strong>No brīnumiem līdz kultūrām</strong>: Septiņi pasaules brīnumi ir saistīti ar senajām civilizācijām, piemēram, ķēniša Babylonas ziedu dārziem, kas bija lielisks inženierijas paraugs.</p>
            </li>
            <li>
                <p><strong>Kalnu ekosistēmas</strong> – augstajos kalnos dzīvotāji ir pieraduši pie īpašiem apstākļiem, piemēram, zemas temperatūras, vāja skābekļa un stipriem vējiem. Kalnu faunā un florā ir daudzas unikālas sugas, piemēram, sniega leopardi un īpaši pielāgotas augu sugas.</p>
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
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/9i0vkz.jpg" />
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
