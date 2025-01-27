<!DOCTYPE html>
<html lang="lv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Attēlu Galerija</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        h1 {
            text-align: center;
            margin: 20px 0;
            color: #333;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            padding: 15px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
        }

        .gallery img:hover {
            transform: scale(1.05);
        }

        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.9);
            display: flex;
            justify-content: center;
            align-items: center;
            visibility: hidden;
            opacity: 0;
            transition: opacity 0.3s ease, visibility 0.3s ease;
        }

        .overlay img {
            max-width: 90%;
            max-height: 90%;
            border-radius: 8px;
            box-shadow: 0px 8px 16px rgba(255, 255, 255, 0.2);
        }

        .overlay.active {
            visibility: visible;
            opacity: 1;
        }

        .overlay:hover {
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Attēlu Galerija</h1>
    <div class="gallery">
        <!-- Attēli tiks ģenerēti ar JavaScript -->
    </div>
    <div class="overlay" id="overlay">
        <img src="" alt="Pilnekrāna attēls">
    </div>
    <script>
        const imageFiles = [
            "https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/a89449563a742c910a117f190694936ac9f25790/Image/attels1.jpg",
            "https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/a89449563a742c910a117f190694936ac9f25790/Image/attels2.jpg",
            "https://raw.githubusercontent.com/ropciko112/Laikrakstsanta/a89449563a742c910a117f190694936ac9f25790/Image/attels3.jpg"
            // Pievieno vairāk attēlu URL pēc nepieciešamības
        ];

        const gallery = document.querySelector('.gallery');
        const overlay = document.getElementById('overlay');
        const overlayImage = overlay.querySelector('img');

        // Pievieno attēlus galerijai
        imageFiles.forEach((src) => {
            const img = document.createElement('img');
            img.src = src;
            img.alt = "Attēls";
            img.addEventListener('click', () => {
                overlayImage.src = src;
                overlay.classList.add('active');
            });
            gallery.appendChild(img);
        });

        // Slēdz pilnekrāna skatu
        overlay.addEventListener('click', () => {
            overlay.classList.remove('active');
        });
    </script>
</body>
</html>
