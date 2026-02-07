<!DOCTYPE html>
<html lang="cs">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developerský projekt</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            color: #222;
        }

        /* HERO */
        .hero {
            background: url('hero.jpg') center/cover no-repeat;
            height: 90vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            padding: 20px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        .btn {
            padding: 12px 24px;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            display: inline-block;
        }

        .primary {
            background: #0077ff;
            color: white;
        }

        .secondary {
            background: white;
            color: #0077ff;
        }

        .hero-buttons .btn {
            margin: 10px;
        }

        /* FILTRACE */
        .filter {
            padding: 40px;
            text-align: center;
            background: #f5f5f5;
        }

        .filter form {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .filter select,
        .filter input[type="range"] {
            padding: 10px;
            font-size: 1rem;
        }

        /* PROJEKTY */
        .projects {
            padding: 60px 20px;
            text-align: center;
        }

        .project-grid {
            display: flex;
            gap: 30px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .project-card {
            width: 300px;
            border-radius: 8px;
            overflow: hidden;
            background: #fff;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            text-align: left;
        }

        .project-card img {
            width: 100%;
        }

        .project-card h3 {
            margin: 15px;
        }

        .project-card p {
            margin: 0 15px 20px;
            color: #555;
        }

        /* BENEFITY */
        .benefits {
            padding: 60px 20px;
            background: #fafafa;
            text-align: center;
        }

        .benefit-grid {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
        }

        .benefit-item {
            max-width: 250px;
        }

        /* FOOTER */
        footer {
            padding: 30px;
            text-align: center;
            background: #222;
            color: white;
        }
    </style>
</head>

<body>

    <!-- HERO -->
    <header class="hero">
        <div>
            <h1>Moderní bydlení pro budoucnost</h1>
            <p>Prémiové projekty v nejžádanějších lokalitách.</p>
            <div class="hero-buttons">
                <a href="#projekty" class="btn primary">Prohlédnout projekty</a>
                <a href="#kontakt" class="btn secondary">Kontaktovat</a>
            </div>
        </div>
    </header>

    <!-- FILTRACE -->
    <section class="filter">
        <h2>Najděte svůj nový domov</h2>
        <form>
            <select>
                <option>Lokalita</option>
                <option>Praha 4</option>
                <option>Praha 5</option>
                <option>Praha 9</option>
            </select>

            <select>
                <option>Dispozice</option>
                <option>1+kk</option>
                <option>2+kk</option>
                <option>3+kk</option>
                <option>4+kk</option>
            </select>

            <input type="range" min="3000000" max="20000000" value="8000000">
            <button class="btn primary">Filtrovat</button>
        </form>
    </section>

    <!-- PROJEKTY -->
    <section id="projekty" class="projects">
        <h2>Aktuální projekty</h2>

        <div class="project-grid">

            <div class="project-card">
                <img src="project1.jpg" alt="Projekt 1">
                <h3>Rezidence Park</h3>
                <p>Praha 5 • od 6 500 000 Kč</p>
            </div>

            <div class="project-card">
                <img src="project2.jpg" alt="Projekt 2">
                <h3>Byty U Řeky</h3>
                <p>Praha 9 • od 5 900 000 Kč</p>
            </div>

            <div class="project-card">
                <img src="project3.jpg" alt="Projekt 3">
                <h3>Moderní čtvrť</h3>
                <p>Praha 4 • od 7 200 000 Kč</p>
            </div>

        </div>
    </section>

    <!-- BENEFITY -->
    <section class="benefits">
        <h2>Proč si vybrat nás</h2>
        <div class="benefit-grid">
            <div class="benefit-item">
                <h3>30 let zkušeností</h3>
                <p>Stovky dokončených projektů.</p>
            </div>
            <div class="benefit-item">
                <h3>Energeticky úsporné domy</h3>
                <p>Moderní technologie a nízké náklady.</p>
            </div>
            <div class="benefit-item">
                <h3>Certifikace kvality</h3>
                <p>BREEAM, WELL a další.</p>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer id="kontakt">
        <p>© 2026 Developerská společnost</p>
        <p>Email: info@developer.cz • Tel: +420 777 123 456</p>
    </footer>

</body>
</html>
