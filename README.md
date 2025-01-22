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
        <p>Šodien vārda dienas svin Rebeka.</p>
    </div>

    <!-- Interesanti fakti -->
    <div id="fakti" class="section">
        <h3>Interesanti fakti par Bioluminiscenci</h3>
        <ul class="facts-list">
          <p><strong>Bioluminiscence ir dabīgā gaismas ražo&scaron;ana</strong>: Bioluminiscence ir gaismas izdalī&scaron;anās no dzīvām būtnēm, un to var novērot gan dzīvniekos, gan mikroorganismos, gan dažās augu sugās.</p>
</li>
<li>
<p><strong>Bioluminiscence rodas ķīmisku reakciju rezultātā</strong>: &Scaron;o gaismu rada ķīmiska reakcija starp enzīmu luciferāzi un substrātu luciferīnu, kuras rezultātā tiek izdalīta gaisma. Reakcija notiek bez siltuma izdalī&scaron;anās (tā sauktais aukstais gaismas veids).</p>
</li>
<li>
<p><strong>Jūras dzīvnieki ir galvenie bioluminiscences īpa&scaron;nieki</strong>: Daudzas jūras dzīvnieku sugas, piemēram, dziļjūras zivis, medūzas un garneles, izmanto bioluminiscenci gan medībās, gan aizsardzībā.</p>
</li>
<li>
<p><strong>Bioluminiscences loma ekosistēmā</strong>: Dzīvnieki izmanto bioluminiscenci, lai piesaistītu partnerus, vilinātu upurus vai aizsargātu sevi. Piemēram, dažas zivis izstaro gaismu, lai &ldquo;izkrāptu&rdquo; citas sugas.</p>
</li>
<li>
<p><strong>Bioluminiscence uzkrājas līdz ar dziļumu</strong>: Jo dziļākā jūrā atrodas dzīvnieks, jo biežāk viņi izmanto bioluminiscenci. Dziļjūras dzīvniekiem bieži vien ir pat spilgtas gaismas izstarotājas, lai izdzīvotu tum&scaron;ajās dziļās ūdeņos.</p>
</li>
<li>
<p><strong>Bioluminiscences izmanto&scaron;ana cilvēku interesēs</strong>: Zinātnieki pēta bioluminiscenci, lai attīstītu jaunas tehnoloģijas, piemēram, gaismas avotus, kas darbojas ar bioloģiskiem mehānismiem vai bioluminiscējo&scaron;as &scaron;ūnas, kas var palīdzēt izsekot audzēju attīstībai.</p>
</li>
<li>
<p><strong>Zinātniski svarīgas bioluminiscējo&scaron;as vielas</strong>: Bioluminiscējo&scaron;as vielas tiek izmantotas arī bioloģiskajās pētniecībās, piemēram, bioluminiscējo&scaron;ās olbaltumvielas tiek izmantotas, lai pētītu &scaron;ūnu funkcijas un molekulāro uzbūvi.</p>
</li>
<li>
<p><strong>Bioluminiscence uz Zemes ir ļoti sena parādība</strong>: Pirmie pierādījumi par bioluminiscenci ir vairāk nekā 500 miljonus gadus veci, kas liecina, ka tā pastāv jau kop&scaron; dzīvības sākuma uz Zemes.</p>
</li>
<li>
<p><strong>Bioluminiscējo&scaron;ie organismi dažreiz izmanto arī ķimikālijas</strong>: Daži dzīvnieki bioluminiscenci izmanto kā aizsardzības mehānismu, piemēram, tādas zivis kā kalmāri izstaro gaismu, lai sajauktu plēsoņu orientē&scaron;anos.</p>
</li>
<li>
<p><strong>Zinātnieki pēta iespējas bioluminiscences izmanto&scaron;anai ārpus Zemes</strong>: Bioluminiscences mehānismi var būt noderīgi ārpus Zemes pētniecībā, jo to izmanto&scaron;ana palīdzētu dzīvotspējīgiem organismiem izdzīvot planētu vidē ar ļoti zemu gaismas līmeni.</p></li>
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
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/9hlyy8.jpg" />
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
