<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laikraksts ANTA</title>
    <style>
        /* Jūsu CSS stili šeit */
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
        <a href="./galerija.html" target="_blank">Galerija</a>
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
            <!-- Jūsu fakti šeit -->
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
        <img class="footer-image" src="./images/9i0vkz.jpg" alt="Dienas joks">
    </div>

    <footer>
        <p class="footer-text-center">&copy; 2025 Laikraksts ANTA. Visas tiesības aizsargātas. PS: Lapa ir domāta kā joks un nav jāuztver nopietni!</p>
    </footer>

    <script src="./script.js" type="text/javascript"></script>
</body>
</html>
