<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet"> <!-- Google Fonts: Roboto -->
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
            text-align: center; /* Virsraksts centrēts */
        }

        header p {
            font-size: 1.2em;
            font-style: italic;
            color: #6e4b3a;
        }

        .header-left, .header-right {
            font-size: 1em;
            color: #5a3d2f;
            text-transform: lowercase; /* Maizi burtiem */
            font-weight: normal;
        }

        /* Jaunās sadaļas */
        .section {
            margin-top: 30px;
            padding: 20px;
            background-color: #f7f7f7;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); /* Pievienots ēnas efekts */
        }

        .section h3 {
            font-family: 'Roboto', sans-serif; /* Izmanto jauno fontu */
            font-size: 2.2em;
            color: #4a2c1b;
            font-weight: 700; /* Biezāki burti */
            text-align: center;
            margin-bottom: 10px;
        }

        .section p {
            font-size: 1.1em;
            color: #5a3d2f;
            line-height: 1.6;
        }

        /* Sadaļa "Vārda diena" neatkarīgi */
        .section-varda-diena h3 {
            text-align: left; /* "Vārda dienas" sadaļas nosaukums pa kreisi */
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
            max-width: 400px; /* Lielāks attēls */
            height: auto;
            border: 3px solid #5a3d2f;
            border-radius: 8px;
        }

        /* Stilizēt "Dienas Joks" tekstu virs attēla */
        .footer-joke-text {
            font-family: 'Roboto', sans-serif; /* Roboto fonta izmantošana */
            font-size: 2.5em; /* Lielāks fonta izmērs */
            color: #5a3d2f; /* Krāsa - tumši brūna */
            font-weight: bold; /* Biezāki burti */
            text-align: center;
            text-transform: uppercase; /* Rakstīt tikai lielajiem burtiem */
            letter-spacing: 3px; /* Pievienots atstarpe starp burtiem */
            margin-bottom: 15px; /* Attālums no attēla */
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Pievienota ēna tekstam */
        }

    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 4</div> <!-- Numurs kreisajā pusē -->
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">17. janvāris, 2025</div> <!-- Datums labajā pusē -->
    </header>

    <!-- Vārda dienas sadaļa -->
    <div class="section section-varda-diena">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienu svin: Tenis, Dravis</p>
    </div>

    <!-- Jaunās sadaļas -->
    <div class="section">
 <h3>Interesanti fakti par grāmatvedību</h3>
<ul>
    <li><strong>Grāmatvedība ir sena profesija:</strong> Grāmatvedība ir viena no vecākajām profesijām pasaulē, kas izsekojama līdz pat senajiem Babilonijas un ēģiptiešu laikiem. Tās pamatprincipi, piemēram, ienākumu un izdevumu uzskaites veidi, ir radīti jau pirms vairāk nekā 5 000 gadiem.</li>
    <li><strong>Dubultā ieraksta sistēma:</strong> Grāmatvedības pamatprincipu veido "dubultā ieraksta" sistēma, kuru 1494. gadā iepazīstināja itāļu matemātiķis un mācītājs Luka Pacioli. Katrs grāmatvedības darījums tiek ierakstīts divos kontos - debetā un kreditā.</li>
    <li><strong>Grāmatvedība un nodokļi:</strong> Grāmatveži bieži ir atbildīgi par nodokļu aprēķināšanu un nomaksu. Viņi izseko uzņēmuma ienākumiem un izdevumiem, lai nodrošinātu, ka tiek ievēroti visi nodokļu likumi un noteikumi.</li>
    <li><strong>Starptautiskie grāmatvedības standarti:</strong> Ar globalizāciju ir pieaudzis nepieciešamība pēc vienotiem grāmatvedības standartiem. Starptautiskie grāmatvedības standarti (IFRS) ir kļuvuši par būtisku instrumentu uzņēmumu finanšu pārskatu sagatavošanā visā pasaulē.</li>
    <li><strong>Grāmatvedība un tehnoloģijas:</strong> Mūsdienās grāmatvedība ir cieši saistīta ar tehnoloģijām. Arvien vairāk tiek izmantotas automatizētas grāmatvedības programmas un mākoņdatošanas risinājumi, lai veiktu uzskaiti un sagatavotu finanšu pārskatus.</li>
    <li><strong>Grāmatvedība palīdz uzņēmuma vadīšanā:</strong> Grāmatvedība nav tikai par finanšu uzskaiti. Tā ir svarīga uzņēmuma vadības sastāvdaļa, kas palīdz pieņemt lēmumus par izdevumiem, investīcijām un izaugsmi.</li>
    <li><strong>Grāmatvedība un uzņēmuma dzīvotspēja:</strong> Uzņēmumi, kuriem nav skaidri noteiktas grāmatvedības procedūras, bieži vien saskaras ar finanšu problēmām. Pareiza grāmatvedība palīdz uzņēmumiem nodrošināt savu finansiālo dzīvotspēju un sekmē izaugsmi.</li>
    <li><strong>Grāmatvedība un budžetēšana:</strong> Grāmatvedība ir būtiska sastāvdaļa arī budžeta plānošanā. Ar precīzu uzskaiti var saprast, kā nauda tiek tērēta un kur ir iespējas uzlabot naudas plūsmu.</li>
</ul>

    </div>

    <!-- Laikapstākļi -->
    <div class="weather">
        <div>
            <h3>Laikapstākļi šodienai</h3>
            <p>Gaisa temperatūra: +5°C</p>
            <p>Debesis: Apmācies, vājš smidzinošs lietus</p>
            <p>Vējš: 3 m/s, DR</p>
        </div>
        <div>
            <h3>Prognoze</h3>
            <p>Vēlāk būs neliels smidzinošs lietus.</p>
        </div>
    </div>

    <!-- Dienas Joks attēls lapas apakšā -->
    <div>
        <div class="footer-joke-text">Dienas Joks</div>
        <img class="footer-image" src="https://i.redd.it/97hzmg9f0kde1.jpeg" alt="Dienas Joks">
    </div>

    <footer>
        <p>&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. Lapa paredzēta kā joks un nav jāuztver nopietni :) </p>
    </footer>
</body>
</html>
