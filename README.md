<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <style>
        body {
            font-family: "Georgia", "Times New Roman", serif;
            background-color: #a1832b;
            margin: 0;
            padding: 0;
            color: #333;
        }

        header {
            background: linear-gradient(135deg, #2c2c2c, #1a1a1a);
            color: white;
            padding: 20px 40px;
            text-align: center;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .header-left {
            font-size: 14px;
        }

        .header-right {
            font-size: 16px;
            text-align: right;
            background-color: rgba(255, 255, 255, 0.1);
            padding: 10px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        h1 {
            font-size: 36px;
            margin: 0;
            font-family: 'Georgia', serif;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        #current-date, #current-time {
            display: block;
            font-size: 16px;
            font-weight: bold;
            color: white;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        nav {
            background-color: #444;
            padding: 15px;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        nav a {
            color: white;
            margin: 0 20px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 16px;
            transition: color 0.3s ease, transform 0.3s ease;
        }

        nav a:hover {
            color: #ddd;
            transform: translateY(-2px);
        }

        .section {
            padding: 30px;
            background-color: white;
            margin: 20px auto;
            border-radius: 12px;
            width: 80%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
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

        #weather {
            background-color: rgba(240, 240, 240, 0.8);
            padding: 15px;
            border-radius: 8px;
            font-size: 18px;
            font-family: 'Georgia', serif;
            border: 1px solid #ccc;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        footer {
            background: linear-gradient(135deg, #2c2c2c, #1a1a1a);
            color: white;
            text-align: center;
            padding: 20px;
            font-family: 'Georgia', serif;
            position: sticky;
            bottom: 0;
            width: 100%;
            z-index: 1000;
            box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.2);
        }

        footer p {
            margin: 0;
            font-size: 18px;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
        }

        .jokes-section {
            padding: 30px;
            background-color: #ffffff;
            margin: 20px auto;
            border-radius: 12px;
            width: 80%;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .jokes-section img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
    </style>
</head>
<body>
    <header>
        <div class="header-left">Nr. 14</div>
        <h1>Laikraksts ANTA</h1>
        <div class="header-right">
            <span id="current-date">Ielādē datumu...</span>
            <span id="current-time">Ielādē laiku...</span>
        </div>
    </header>

    <nav>
        <a href="docs/galerija.html">Galerija</a>
        <a href="docs/game.html">Spēle</a>
    </nav>

    <div style="text-align: center; background-color: #fff; padding: 20px; margin: 20px auto; border-radius: 12px; width: 80%; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);">
        <h3>🎵 Klausies dziesmu "Antas piedzīvojumi"</h3>
        <audio controls>
            <source src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/main/docs/Antas%20piedz%C4%ABvojumi.mp3%20(1)" type="audio/mpeg">
            Jūsu pārlūkprogramma neatbalsta audio atskaņošanu.
        </audio>
    </div>

    <div id="vardadiena" class="section">
        <h3>Vārda diena</h3>
        <p>Šodien vārda dienas svin: Lolita, Vitolds.</p>
    </div>

    <div id="fakti" class="section">
        <h3>Interesanti fakti par: Antu.</h3>
        <ul class="facts-list">
            <li><strong>Antu un Juri IVP kopā sauc par saldo pārīti.</strong></li>
            <li><strong>Antai patīk kad viņu kāds cenšas ievērt durvīs.</strong></li>
            <li><strong>Antas mīļākais ēdiens ir medus kūka.</strong></li>
            <li><strong>Anta nāk uz darbu ātrāk lai varētu paspēlēties ar sunīšu mantiņu.</strong></li>
        </ul>
    </div>

    <div id="laikapstakli" class="section">
        <h3>Laikapstākļi Rīgā</h3>
        <div id="weather">Ielādē laikapstākļus...</div>
    </div>

    <div id="groq-response" class="section">
        <h3>Kas ir ātri valodas modeļi?</h3>
        <p id="groq-answer">Ielādē atbildi...</p>
    </div>

    <div id="joks" class="jokes-section">
        <h3>Dienas Joks</h3>
        <img class="footer-image" src="https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/refs/heads/main/Image/20250416_1136_Kafija%20un%20burk%C4%81ni_remix_01jryvrwbte56s703aad3vx95k.png" />
    </div>

    <footer>
        <p class="footer-text-center">&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. PS: Lapa ir domāta kā joks un nav jāuztver nopietni!</p>
    </footer>

    <script>
        function updateTimeAndDate() {
            const now = new Date();
            const hours = String(now.getHours()).padStart(2, '0');
            const minutes = String(now.getMinutes()).padStart(2, '0');
            const seconds = String(now.getSeconds()).padStart(2, '0');
            const day = String(now.getDate()).padStart(2, '0');
            const month = String(now.getMonth() + 1).padStart(2, '0');
            const year = now.getFullYear();
            document.getElementById('current-time').textContent = `${hours}:${minutes}:${seconds}`;
            document.getElementById('current-date').textContent = `${day}.${month}.${year}`;
        }

        updateTimeAndDate();
        setInterval(updateTimeAndDate, 1000);

        async function getWeather() {
            const apiKey = 'cb3813b33fb4488bbf0201525240506';
            const city = 'Riga';
            try {
                const response = await fetch(`https://api.weatherapi.com/v1/current.json?key=${apiKey}&q=${city}&lang=lv`);
                const data = await response.json();
                const temperature = data.current.temp_c;
                const condition = data.current.condition.text;
                const wind = data.current.wind_kph;

                document.getElementById('weather').innerHTML = `Rīgā šobrīd ir ${temperature}°C, ${condition.toLowerCase()}, vējš ${wind} km/h.`;
            } catch (error) {
                document.getElementById('weather').innerHTML = 'Neizdevās ielādēt laikapstākļus.';
            }
        }

        getWeather();

        async function fetchGroqAnswer() {
            try {
                const response = await fetch('https://api.groq.com/openai/v1/chat/completions', {
                    method: 'POST',
                    headers: {
                        'Content-Type': 'application/json',
                        'Authorization': 'Bearer <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>'
                    },
                    body: JSON.stringify({
                        model: 'llama3-8b-8192',
                        messages: [
                            {
                                role: 'user',
                                content: 'Explain the importance of fast language models.'
                            }
                        ],
                        temperature: 0.7
                    })
                });

                const data = await response.json();
                const reply = data.choices?.[0]?.message?.content || 'Neizdevās iegūt atbildi.';
                document.getElementById('groq-answer').innerText = reply;
            } catch (error) {
                document.getElementById('groq-answer').innerText = 'Neizdevās iegūt atbildi.';
            }
        }

        fetchGroqAnswer();
    </script>
</body>
</html>
