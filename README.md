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
        footer {
            background-color: #d8cfc4;
            text-align: center;
            padding: 15px 0;
            font-size: 0.9em;
            color: #9b7e6f;
            border-top: 2px solid #3e3e3e;
            margin-top: 40px;
        }
        .weather {
            text-align: center;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 5</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">20. janvāris, 2025</div>
    </header>

    <!-- Laikapstākļi sadaļa -->
    <div class="section">
        <h3>Laikapstākļi prognoze Rīgai</h3>
        <div id="weather" class="weather">Ielādē laikapstākļus...</div>
    </div>

    <footer>
        <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. Lapa paredzēta kā joks un nav jāuztver nopietni :)</p>
    </footer>

    <script>
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
                console.error("Kļūda:", error);
                document.getElementById("weather").innerText = "Kļūda, mēģiniet vēlreiz.";
            });
    </script>
</body>
</html>
