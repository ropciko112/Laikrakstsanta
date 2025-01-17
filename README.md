<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Pamatstili avīzes izskatam */
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f4f1e1;
            color: #3e3e3e;
            margin: 0;
            padding: 0;
            line-height: 1.6;
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
        }

        .footer-joke-text {
            font-family: 'Roboto', sans-serif;
            font-size: 2.5em;
            color: #5a3d2f;
            font-weight: bold;
            text-align: center;
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-bottom: 15px;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3);
        }

        .footer-image {
            display: block;
            margin: 40px auto;
            width: 50%;
            max-width: 400px;
            height: auto;
            border: 3px solid #5a3d2f;
            border-radius: 8px;
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

    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 4</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">17. janvāris, 2025</div>
    </header>

    <div class="section">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienu svin: Tenis, Dravis</p>
    </div>

    <div class="section">
        <h3>Interesanti fakti par Piekdienām</h3>
        <ul>
            <li><strong>Nosaukuma izcelsme:</strong> Piektdienas nosaukums daudzās valodās ir saistīts ar mīlestības un skaistuma dievieti. Latviešu valodā "piektdiena" norāda uz piekto nedēļas dienu...</li>
            <li><strong>Piektdiena 13. datums:</strong> Piektdiena, kas iekrīt 13. datumā, tiek uzskatīta par neveiksmīgu dienu...</li>
            <li><strong>Lielā Piektdiena:</strong> Kristīgajā tradīcijā Lielā Piektdiena ir diena, kad piemin Jēzus Kristus krustā sišanu...</li>
            <!-- Citas ziņas šeit -->
        </ul>
    </div>

    <div class="section">
        <h3>Laikapstākļi šodienai</h3>
        <p>Gaisa temperatūra: +5°C</p>
        <p>Debesis: Apmācies, vājš smidzinošs lietus</p>
        <p>Vējš: 3 m/s, DR</p>
    </div>

    <div>
        <div class="footer-joke-text">Dienas Joks</div>
        <img class="footer-image" src="https://i.redd.it/97hzmg9f0kde1.jpeg" alt="Dienas Joks">
    </div>

    <footer>
        <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas.</p>
    </footer>
</body>
</html>
