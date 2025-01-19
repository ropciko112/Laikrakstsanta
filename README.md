<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Pamatstili avīzes izskatam */
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

        /* Galvene */
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

        header p {
            font-size: 1.2em;
            font-style: italic;
            color: #6e4b3a;
        }

        .header-left, .header-right {
            font-size: 1em;
            color: #5a3d2f;
            text-transform: lowercase;
            font-weight: normal;
        }

        /* Jaunās sadaļas */
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

        /* Sadaļa "Vārda diena" */
        .section-varda-diena h3 {
            text-align: left;
            font-size: 2em;
            color: #4a2c1b;
            margin-bottom: 10px;
        }

        /* Kājene */
        footer {
            background-color: #d8cfc4;
            text-align: center;
            padding: 15px 0;
            font-size: 0.9em;
            color: #9b7e6f;
            border-top: 2px solid #3e3e3e;
            margin-top: 40px;
        }

        /* Attēls lapas apakšā */
        .footer-image {
            display: block;
            margin: 40px auto;
            width: 50%;
            max-width: 400px;
            height: auto;
            border: 3px solid #5a3d2f;
            border-radius: 8px;
        }

    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 5</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">20. janvāris, 2025</div>
    </header>

    <!-- Vārda dienas sadaļa -->
    <div class="section section-varda-diena">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienu svin: Oļģerts, Orests, Aļģirds, Aļģis.</p>
    </div>

    <!-- Jaunās sadaļas -->
    <div class="section">
        <h3>Interesanti fakti par grāmatvedību</h3>
        <ul>
            <li><strong>Grāmatvedība ir sena profesija:</strong> Grāmatvedība ir viena no vecākajām profesijām pasaulē, kas izsekojama līdz pat senajiem Babilonijas un ēģiptiešu laikiem. Tās pamatprincipi, piemēram, ienākumu un izdevumu uzskaites veidi, ir radīti jau pirms vairāk nekā 5 000 gadiem.</li>
            <li><strong>Dubultā ieraksta sistēma:</strong> Grāmatvedības pamatprincipu veido "dubultā ieraksta" sistēma, kuru 1494. gadā iepazīstināja itāļu matemātiķis un mācītājs Luka Pacioli. Katrs grāmatvedības darījums tiek ierakstīts divos kontos - debetā un kreditā.</li>
            <!-- citi fakti -->
        </ul>
    </div>

    <!-- Laikapstākļi -->
    <div class="widget widget-weather-parameters js-dataset widget-oneday widget-tomorrow">
        <div>
            <h3>Laikapstākļi šodienai</h3>
            <p id="temperature">Gaisa temperatūra: ...</p>
            <p id="description">Debesis: ...</p>
            <p id="wind">Vējš: ...</p>
        </div>
        <div>
            <h3>Prognoze</h3>
            <p id="forecast">...Prognoze tiek iegūta...</p>
        </div>
    </div>

    <!-- Jaunais attēls -->
    <div>
        <img class="footer-image" src="https://i.redd.it/nza8lhmtjzde1.jpeg" alt="u/Low-Sir-7440 - vins">
    </div>

    <footer>
        <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. Lapa paredzēta kā joks un nav jāuztver nopietni :)</p>
    </footer>

    <script>
        // OpenWeatherMap API atslēga
        const apiKey = 'TAVA_API_ATSLEGA'; // Aizvieto ar savu API atslēgu
        const city = 'Riga'; // Izvēlies pilsētu

        // Funkcija, lai iegūtu laikapstākļus no API
        function getWeather() {
            fetch(`https://api.openweathermap.org/data/2.5/weather?q=${city}&units=metric&lang=lv&appid=${apiKey}`)
                .then(response => response.json())
                .then(data => {
                    // Atjaunojam datus HTML lapā
                    document.getElementById('temperature').innerText = `Gaisa temperatūra: ${data.main.temp}°C`;
                    document.getElementById('description').innerText = `Debesis: ${data.weather[0].description}`;
                    document.getElementById('wind').innerText = `Vējš: ${data.wind.speed} m/s`;
                    document.getElementById('forecast').innerText = `Prognoze: ${data.weather[0].description}`;
                })
                .catch(error => {
                    console.error('Kļūda iegūstot laikapstākļus:', error);
                    document.querySelector('.widget').innerHTML = '<p>Neizdevās iegūt laikapstākļus.</p>';
                });
        }

        // Iegūt laikapstākļus pēc lapas ielādes
        window.onload = getWeather;
    </script>

</body>
</html>
