<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PetTrans UK</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-image: url('1.PNG'); /* Imaginea trebuie să fie în același folder */
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            color: #333;
        }
        header {
            background-color: rgba(0, 123, 255, 0.8);
            color: white;
            text-align: center;
            padding: 20px;
            position: sticky;
            top: 0;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        footer {
            text-align: center;
            background: rgba(0, 0, 0, 0.8);
            color: white;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        select {
            margin: 10px;
            padding: 5px;
            font-size: 16px;
        }
        button {
            margin: 5px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 4px;
        }
        button:hover {
            background-color: #0056b3;
        }
    </style>
    <script>
        const translations = {
            en: {
                title: "PetTrans UK",
                subtitle: "Safe Paws, Happy Journeys – We Deliver Trust Across Borders",
                about_title: "About Us",
                about_content: "At PetTrans UK, we provide stress-free, fully insured transport services tailored to your pets' needs.",
                services_title: "Our Services",
                service1: "Door-to-door transportation for dogs and cats",
                service2: "Real-time GPS tracking",
                service3: "Comfortable crates, regular breaks, and hydration",
                pricing_title: "Pricing",
                pricing_content: "Competitive pricing for the best service:",
                dog_price: "Dogs: Starting from £300",
                cat_price: "Cats: Starting from £250",
                contact_title: "Contact Us",
                phone: "Phone/WhatsApp: +44 123 456 7890",
                email: "Email: info@pettransuk.com",
                hours: "Working hours: Monday to Friday, 9 AM to 5 PM",
            },
            ro: {
                title: "PetTrans UK",
                subtitle: "Lăbuțe în siguranță, călătorii fericite – livrăm încredere peste granițe",
                about_title: "Despre Noi",
                about_content: "La PetTrans UK, oferim servicii de transport fără stres, complet asigurate, adaptate nevoilor animalelor de companie.",
                services_title: "Serviciile Noastre",
                service1: "Transport door-to-door pentru câini și pisici",
                service2: "Urmărire GPS în timp real",
                service3: "Cuști confortabile, pauze regulate și hidratare",
                pricing_title: "Prețuri",
                pricing_content: "Prețuri competitive pentru cele mai bune servicii:",
                dog_price: "Câini: De la £300",
                cat_price: "Pisici: De la £250",
                contact_title: "Contactați-ne",
                phone: "Telefon/WhatsApp: +44 123 456 7890",
                email: "Email: info@pettransuk.com",
                hours: "Program de lucru: Luni-Vineri, 9 AM - 5 PM",
            }
        };

        function changeLanguage() {
            const lang = document.getElementById("language").value;
            for (const key in translations[lang]) {
                const element = document.getElementById(key);
                if (element) {
                    element.innerText = translations[lang][key];
                }
            }
        }
    </script>
</head>
<body>
    <header>
        <h1 id="title">PetTrans UK</h1>
        <p id="subtitle">Safe Paws, Happy Journeys – We Deliver Trust Across Borders</p>
        <select id="language" onchange="changeLanguage()">
            <option value="en">English</option>
            <option value="ro">Română</option>
        </select>
    </header>
    <div class="container">
        <section>
            <h2 id="about_title">About Us</h2>
            <p id="about_content">At PetTrans UK, we provide stress-free, fully insured transport services tailored to your pets' needs.</p>
        </section>
        <section>
            <h2 id="services_title">Our Services</h2>
            <ul>
                <li id="service1">Door-to-door transportation for dogs and cats</li>
                <li id="service2">Real-time GPS tracking</li>
                <li id="service3">Comfortable crates, regular breaks, and hydration</li>
            </ul>
        </section>
        <section>
            <h2 id="pricing_title">Pricing</h2>
            <p id="pricing_content">Competitive pricing for the best service:</p>
            <ul>
                <li id="dog_price">Dogs: Starting from £300</li>
                <li id="cat_price">Cats: Starting from £250</li>
            </ul>
        </section>
        <section>
            <h2 id="contact_title">Contact Us</h2>
            <p id="phone">Phone/WhatsApp: +44 123 456 7890</p>
            <p id="email">Email: info@pettransuk.com</p>
            <p id="hours">Working hours: Monday to Friday, 9 AM to 5 PM</p>
