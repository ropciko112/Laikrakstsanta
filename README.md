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
        <div class="header-left">Nr. 9</div>
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
        <p>Šodien vārda dienas svin: Krišs, Ksenija, Eglons, Egle.</p>
    </div>

    <!-- Interesanti fakti -->
    <div id="fakti" class="section">
        <h3>Interesanti fakti par: Pasaules augstākiem kalniem.</h3>
        <ul class="facts-list">
          <p><strong>Everests nav vienīgais augstākais kalns</strong> &ndash; lai gan Mount Everest ir augstākais kalns uz Zemes, ja ņem vērā tikai kalnus, kas mēra no jūras līmeņa, tad <strong>Mauna Kea</strong> Havaju salās, kas sākas no okeāna dibena, faktiski ir augstākais kalns pasaulē, ar kopējo augstumu 10 210 metru.</p>
<li>
<p><strong>Everesta augstums nemainās ievērojami</strong> &ndash; Mount Everest augstums tiek regulāri pārbaudīts, un pēdējais noteiktais augstums ir 8 848,86 metri, kas tika apstiprināts 2020. gadā pēc kopīgiem ķīnie&scaron;u un nepālie&scaron;u pētījumiem.</p>
</li>
<li>
<p><strong>Zemākās un augstākās vietas uz Zemes</strong> &ndash; ja runājam par zemākajiem un augstākajiem punktiem uz Zemes, tad <strong>Everests</strong> ir augstākais, savukārt <strong>Nāves jūra</strong> ir viena no zemākajām vietām, tās virsma ir 430 metrus zem jūras līmeņa.</p>
</li>
<li>
<p><strong>Altitūdā cilvēka ķermenis reaģē</strong> &ndash; augstākos kalnos, piemēram, Everestā, ir ļoti zems skābekļa līmenis, kas var izraisīt <strong>augstuma slimību</strong>. Lai to novērstu, kalnos kāpējiem jāveic aklimatizācijas procesi, un dažreiz viņiem jāizmanto skābekļa baloni.</p>
</li>
<li>
<p><strong>Kalnu kāp&scaron;anas vēsture</strong> &ndash; pirmā dokumentētā Everestā sasniegtā virsotne bija 1953. gadā, kad sir Edmunds Hillary no Jaunzēlandes un Tenzings Norgays no Nepālas uzkāpa kalnā. Tomēr līdz tam kalns jau bija bijis zināms, un vairāki pētījumi un mēģinājumi tika veikti vēl pirms tam.</p>
</li>
<li>
<p><strong>Kāpinājumi un izaicinājumi</strong> &ndash; Mount Everesta kāp&scaron;ana ir liels izaicinājums, ne tikai fizioloģiski, bet arī morāli. Katru gadu uz Everestu dodas tūksto&scaron;iem cilvēku, taču daudzi no viņiem cie&scaron; no smagām slimībām vai mirst augstuma dēļ, kas padara &scaron;o kāp&scaron;anu par ļoti bīstamu.</p>
</li>
<li>
<p><strong>Kāpēju "josla"</strong> &ndash; virs 8 000 metriem atrodas tā dēvētais "nāves zonu", kur cilvēkiem ir ļoti grūti izdzīvot bez papildus skābekļa. &Scaron;ajā augstumā skābekļa daudzums ir tikai aptuveni 1/3 no zemākas altitūdas līmeņa.</p>
</li>
<li>
<p><strong>Mērījumu precizitāte</strong> &ndash; kalnu augstums tiek mērīts, izmantojot dažādas tehnoloģijas, piemēram, satelītus, GPS un trigonometriju, un tās kļūdas var būt mazākas par dažiem centimetriem.</p>
</li>
<li>
<p><strong>Citi ievērojami kalni</strong> &ndash; daži no citiem ievērojamiem kalniem pasaulē ir K2 (8 611 metri), Kangchenjunga (8 586 metri), Lhotse (8 516 metri) un Makalu (8 485 metri).</p>
</li>
<li>
<p><strong>Kalnu ekosistēmas</strong> &ndash; augstajos kalnos dzīvotāji ir pieradu&scaron;i pie īpa&scaron;iem apstākļiem, piemēram, zemas temperatūras, vāja skābekļa un stipriem vējiem. Kalnu faunā un florā ir daudzas unikālas sugas, piemēram, sniega leopardi un īpa&scaron;i pielāgotas augu sugas.</p></li>
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
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/9hpxoo.jpg" />
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
