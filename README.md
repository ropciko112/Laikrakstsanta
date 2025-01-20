<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Times New Roman', serif;
            background-color: #f4f1e1;
            color: #3e3e3e;
            margin: 0;
            padding: 0;
        }
        h1, h2, h3, p {
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #d8cfc4;
            padding: 20px 10px;
            text-align: center;
            border-bottom: 2px solid #3e3e3e;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        header h1 {
            font-size: 3.5em;
            text-transform: uppercase;
            color: #5a3d2f;
            letter-spacing: 5px;
            flex: 1;
            text-align: center;
        }
        .header-left, .header-right {
            font-size: 1em;
            color: #5a3d2f;
        }
        .section {
            margin-top: 30px;
            padding: 20px;
            background-color: #f7f7f7;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .section h3 {
            font-family: 'Roboto', sans-serif;
            font-size: 2.2em;
            color: #4a2c1b;
            font-weight: 700;
            text-align: center;
            margin-bottom: 10px;
        }
        .section p {
            font-size: 1.1em;
            color: #5a3d2f;
            line-height: 1.6;
        }
        ul.facts-list {
            list-style-type: decimal;
            margin-left: 20px;
        }
        footer {
            background-color: #d8cfc4;
            text-align: center;
            padding: 15px 0;
            font-size: 0.9em;
            color: #9b7e6f;
            border-top: 2px solid #3e3e3e;
            margin-top: 40px;
        }
        /* Jauni stili dienas jokam */
        .footer-joke-text {
            font-size: 1.5em;
            color: #4a2c1b;
            font-weight: 700;
            margin-top: 30px;
            text-align: center;
        }
        .footer-image {
            display: block;
            margin: 20px auto;
            width: 80%;
            max-width: 500px;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 5</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right"><span id="current-time">Ielādē laiku...</span></div>
    </header>

    <!-- Vārda diena -->
    <div class="section">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienu svin: Oļģerts, Orests, Aļģirds, Aļģis.</p>
    </div>

    <!-- Interesanti fakti -->
    <div class="section">
        <h3>Interesanti fakti par grāmatvedību</h3>
        <ul class="facts-list">
            <li><strong>Grāmatvedība ir sena profesija:</strong> Grāmatvedība ir viena no vecākajām profesijām pasaulē, kas izsekojama līdz pat senajiem Babilonijas un ēģiptiešu laikiem.</li>
            <li><strong>Dubultā ieraksta sistēma:</strong> Grāmatvedības pamatprincipu veido "dubultā ieraksta" sistēma, kuru 1494. gadā iepazīstināja itāļu matemātiķis un mācītājs Luka Pacioli.</li>
            <li><strong>Grāmatvedība un nodokļi:</strong> Grāmatveži bieži ir atbildīgi par nodokļu aprēķināšanu un nomaksu, nodrošinot uzņēmumu atbilstību likumiem.</li>
            <li><strong>Starptautiskie grāmatvedības standarti:</strong> Starptautiskie grāmatvedības standarti (IFRS) tiek izmantoti uzņēmumu finanšu pārskatu sagatavošanai globālā mērogā.</li>
            <li><strong>Grāmatvedība un tehnoloģijas:</strong> Mūsdienās grāmatvedība ir cieši saistīta ar tehnoloģijām, un arvien vairāk tiek izmantotas automatizētas grāmatvedības programmas.</li>
            <li><strong>Grāmatvedība palīdz uzņēmuma vadīšanā:</strong> Grāmatvedība ir svarīga uzņēmuma vadības sastāvdaļa, kas palīdz pieņemt lēmumus par izdevumiem, investīcijām un izaugsmi.</li>
            <li><strong>Grāmatvedība un uzņēmuma dzīvotspēja:</strong> Pareiza grāmatvedība palīdz uzņēmumiem nodrošināt savu finansiālo dzīvotspēju un sekmē izaugsmi.</li>
            <li><strong>Grāmatvedība un budžetēšana:</strong> Grāmatvedība ir būtiska sastāvdaļa arī budžeta plānošanā, kas palīdz saprast, kā nauda tiek tērēta un kur ir iespējas uzlabot naudas plūsmu.</li>
            <li><strong>Grāmatvedība un finanšu pārskati:</strong> Grāmatvedība veido pamatu uzņēmumu finanšu pārskatiem, kas palīdz noteikt uzņēmuma peļņu vai zaudējumus.</li>
            <li><strong>Grāmatvedība un nākotnes prognozes:</strong> Grāmatveži izmanto datus, lai veiktu prognozes un palīdzētu uzņēmumiem plānot nākotnes izdevumus un ienākumus.</li>
        </ul>
    </div>

    <!-- Laikapstākļi -->
    <div class="section">
        <h3>Laikapstākļi Rīgā</h3>
        <div id="weather">Ielādē laikapstākļus...</div>
    </div>

    <!-- Dienas Joks -->
    <div>
        <div class="footer-joke-text">Dienas Joks</div>
        <img class="footer-image" src="https://i.redd.it/nza8lhmtjzde1.jpeg" alt="u/Low-Sir-7440 - vins">
    </div>

    <footer>
        <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas.</p>
    </footer>

    <script>
        // Reāllaika pulkstenis
        function updateTime() {
            const now = new Date();
            document.getElementById('current-time').textContent = now.toLocaleTimeString('lv-LV');
        }
        setInterval(updateTime, 1000);
        updateTime();

        // Laikapstākļu prognoze
        const apiKey = "1b5e2264709b5eacd217f25ebf6dc09a";
        const city = "Riga";
        const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}&units=metric&lang=lv`;

        fetch(apiUrl)
            .then(response => response.json())
            .then(data => {
                if (data.cod === 200) {
                    const weatherDiv = document.getElementById("weather");
                    weatherDiv.innerHTML = `
                        <p><strong>Pilsēta:</strong> ${data.name}</p>
                        <p><strong>Temperatūra:</strong> ${data.main.temp} °C</p>
                        <p><strong>Laikapstākļi:</strong> ${data.weather[0].description}</p>
                        <p><strong>Vēja ātrums:</strong> ${data.wind.speed} m/s</p>
                    `;
                } else {
                    document.getElementById("weather").innerText = "Neizdevās ielādēt laikapstākļus.";
                }
            })
            .catch(error => {
                document.getElementById("weather").innerText = "Kļūda, mēģiniet vēlreiz.";
            });
    </script>
</body>
</html>
