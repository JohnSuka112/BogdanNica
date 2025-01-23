
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PetTrans UK - Safe Pet Transport</title>
    <style>
        background-image: url('https://github.com/JohnSuka112/BogdanNica/blob/dffce38004ef36d672a1a541775cc05c05f863ca/4E7D3A83-4CC6-492F-B29D-008ECD740E6F.PNG');
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('A_visually_captivating_background_featuring_a_frie.png');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
        }
        header {
            background-color: rgba(0, 123, 255, 0.8);
            color: white;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            margin: 0;
        }
        nav {
            background-color: rgba(0, 86, 179, 0.8);
            color: white;
            padding: 10px;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .language-selector {
            position: absolute;
            top: 20px;
            right: 20px;
        }
        .language-selector select {
            padding: 5px;
            font-size: 16px;
        }
        section {
            padding: 20px;
            margin: 10px auto;
            max-width: 800px;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        footer {
            background-color: rgba(52, 58, 64, 0.9);
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <div class="language-selector">
        <label for="language">Language:</label>
        <select id="language" onchange="changeLanguage()">
            <option value="en">English</option>
            <option value="ro">Română</option>
        </select>
    </div>
    <header>
        <h1 id="title">PetTrans UK</h1>
        <p id="subtitle">Safe Paws, Happy Journeys – We Deliver Trust Across Borders</p>
    </header>
    <nav>
        <a href="#about" id="nav-about">About Us</a>
        <a href="#services" id="nav-services">Services</a>
        <a href="#pricing" id="nav-pricing">Pricing</a>
        <a href="#contact" id="nav-contact">Contact</a>
    </nav>
    <section id="about">
        <h2 id="about-title">About Us</h2>
        <p id="about-content">At PetTrans UK, we understand that pets are family. That’s why we provide stress-free, fully insured transport services tailored to their needs. Our experienced team ensures the journey is safe, comfortable, and timely.</p>
    </section>
    <section id="services">
        <h2 id="services-title">Our Services</h2>
        <ul>
            <li id="service1">Door-to-door transportation for dogs and cats</li>
            <li id="service2">Real-time GPS tracking</li>
            <li id="service3">Comfortable crates, regular breaks, and hydration</li>
        </ul>
    </section>
    <section id="pricing">
        <h2 id="pricing-title">Pricing</h2>
        <p id="pricing-content">We offer competitive pricing to ensure the best service for your pets:</p>
        <ul>
            <li id="dog-price"><strong>Dogs:</strong> Starting from £300</li>
            <li id="cat-price"><strong>Cats:</strong> Starting from £250</li>
        </ul>
        <p id="discount">Discounts available for multiple pets!</p>
    </section>
    <section id="contact">
        <h2 id="contact-title">Contact Us</h2>
        <p id="phone"><strong>Phone/WhatsApp:</strong> +44 123 456 7890</p>
        <p id="email"><strong>Email:</strong> info@pettransuk.com</p>
        <p id="hours"><strong>Working hours:</strong> Monday-Saturday, 9:00 AM – 6:00 PM</p>
    </section>
    <footer>
        <p>&copy; 2025 PetTrans UK. All Rights Reserved.</p>
    </footer>
    <script>
        const translations = {
            "ro": {
                "title": "PetTrans UK",
                "subtitle": "Lăbuțe în siguranță, călătorii fericite – Livrăm încredere peste granițe",
                "nav-about": "Despre Noi",
                "nav-services": "Servicii",
                "nav-pricing": "Prețuri",
                "nav-contact": "Contact",
                "about-title": "Despre Noi",
                "about-content": "La PetTrans UK, înțelegem că animalele de companie sunt familie. De aceea oferim servicii de transport fără stres, complet asigurate, adaptate nevoilor lor. Echipa noastră experimentată asigură o călătorie sigură, confortabilă și la timp.",
                "services-title": "Serviciile Noastre",
                "service1": "Transport de la ușă la ușă pentru câini și pisici",
                "service2": "Urmărire GPS în timp real",
                "service3": "Cuști confortabile, pauze regulate și hidratare",
                "pricing-title": "Prețuri",
                "pricing-content": "Oferim prețuri competitive pentru a asigura cele mai bune servicii pentru animalele dumneavoastră:",
                "dog-price": "<strong>Câini:</strong> De la 300£",
                "cat-price": "<strong>Pisici:</strong> De la 250£",
                "discount": "Reduceri disponibile pentru mai multe animale!",
                "contact-title": "Contact",
                "phone": "<strong>Telefon/WhatsApp:</strong> +44 123 456 7890",
                "email": "<strong>Email:</strong> info@pettransuk.com",
                "hours": "<strong>Ore de lucru:</strong> Luni-Sâmbătă, 9:00 – 18:00"
            },
            "en": {
                // Default values, no changes needed
            }
        };
        
        function changeLanguage() {
            const lang = document.getElementById('language').value;
            const elements = Object.keys(translations[lang]);
            elements.forEach(id => {
                document.getElementById(id).innerHTML = translations[lang][id];
            });
        }
    </script>
</body>
</html>
