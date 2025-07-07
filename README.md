<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta Lanfaala immobilier & Services="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lanfaala Immobilier & Services | Conakry</title>
    <meta name="description" content="Agence immobilière à Conakry spécialisée dans la vente, location et gestion de biens immobiliers.">
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Barre de navigation -->
    <nav>
        <div class="logo">
            <h1>Lanfaala Immobilier</h1>
        </div>
        <ul class="nav-links">
            <li><a href="#accueil">Accueil</a></li>
            <li><a href="#biens">Biens</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
        <div class="burger">
            <i class="fas fa-bars"></i>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="accueil" class="hero">
        <div class="hero-content">
            <h2>Votre partenaire immobilier à Conakry</h2>
            <p>Découvrez des biens exclusifs et un accompagnement sur mesure.</p>
            <a href="#biens" class="btn">Voir nos offres</a>
        </div>
    </section>

    <!-- Section Biens Immobiliers -->
    <section id="biens" class="properties">
        <h2>Nos Biens Disponibles</h2>
        <div class="property-grid">
            <!-- Exemple de carte de bien -->
            <div class="property-card">
                <img src="appartement-conakry.jpg" alt="Appartement à Conakry">
                <div class="property-info">
                    <h3>Appartement R+3, Minière</h3>
                    <p><i class="fas fa-map-marker-alt"></i> Conakry, Guinée</p>
                    <p><i class="fas fa-bed"></i> 3 chambres | <i class="fas fa-bath"></i> 2 salles de bain</p>
                    <p class="price">850.000.000 GNF</p>
                    <a href="#" class="btn">Voir détails</a>
                </div>
            </div>
            <!-- Ajouter d'autres biens ici -->
        </div>
    </section>

    <!-- Section Services -->
    <section id="services" class="services">
        <h2>Nos Services</h2>
        <div class="services-grid">
            <div class="service-card">
                <i class="fas fa-home"></i>
                <h3>Achat & Vente</h3>
                <p>Transaction sécurisée de biens immobiliers.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-key"></i>
                <h3>Location</h3>
                <p>Gestion locative simplifiée.</p>
            </div>
            <div class="service-card">
                <i class="fas fa-building"></i>
                <h3>Gestion de Patrimoine</h3>
                <p>Optimisation de vos investissements.</p>
            </div>
        </div>
    </section>

    <!-- Formulaire de Contact -->
    <section id="contact" class="contact">
        <h2>Contactez-nous</h2>
        <form id="contact-form">
            <input type="text" placeholder="Nom" required>
            <input type="email" placeholder="Email" required>
            <input type="tel" placeholder="Téléphone">
            <textarea placeholder="Votre message" required></textarea>
            <button type="submit" class="btn">Envoyer</button>
        </form>
    </section>

    <!-- Pied de page -->
    <footer>
        <div class="footer-content">
            <div class="footer-logo">
                <h3>Lanfaala Immobilier & Services</h3>
                <p>Votre confort, notre priorité.</p>
            </div>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-whatsapp"></i></a>
            </div>
        </div>
        <p class="copyright">&copy; 2024 Lanfaala Immobilier. Tous droits réservés.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
/* Reset & Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

body {
    line-height: 1.6;
    color: #333;
}

/* Navigation */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 5%;
    background: #fff;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    position: fixed;
    width: 100%;
    z-index: 1000;
}

.logo h1 {
    color: #2c3e50;
    font-weight: 700;
}

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li a {
    margin-left: 2rem;
    text-decoration: none;
    color: #2c3e50;
    font-weight: 500;
}

.burger {
    display: none;
    cursor: pointer;
}

/* Hero Section */
.hero {
    height: 100vh;
    background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('hero-bg.jpg') no-repeat center/cover;
    display: flex;
    align-items: center;
    padding: 0 5%;
    color: #fff;
}

.hero-content h2 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
}

.btn {
    display: inline-block;
    background: #e74c3c;
    color: #fff;
    padding: 0.8rem 1.5rem;
    border: none;
    border-radius: 5px;
    text-decoration: none;
    font-weight: 600;
    transition: background 0.3s;
}

.btn:hover {
    background: #c0392b;
}

/* Property Grid */
.properties {
    padding: 5rem 5%;
}

.properties h2, .services h2, .contact h2 {
    text-align: center;
    margin-bottom: 3rem;
    font-size: 2.5rem;
    color: #2c3e50;
}

.property-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 2rem;
}

.property-card {
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s;
}

.property-card:hover {
    transform: translateY(-10px);
}

.property-card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.property-info {
    padding: 1.5rem;
}

.property-info h3 {
    margin-bottom: 0.5rem;
}

.property-info p {
    margin: 0.5rem 0;
    color: #7f8c8d;
}

.price {
    font-weight: bold;
    color: #e74c3c !important;
    font-size: 1.2rem;
}

/* Services */
.services {
    padding: 5rem 5%;
    background: #f9f9f9;
}

.services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.service-card {
    text-align: center;
    padding: 2rem;
    background: #fff;
    border-radius: 8px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
}

.service-card i {
    font-size: 3rem;
    color: #e74c3c;
    margin-bottom: 1rem;
}

/* Contact Form */
.contact {
    padding: 5rem 5%;
}

#contact-form {
    max-width: 600px;
    margin: 0 auto;
    display: grid;
    gap: 1rem;
}

#contact-form input, #contact-form textarea {
    padding: 0.8rem;
    border: 1px solid #ddd;
    border-radius: 5px;
}

#contact-form textarea {
    resize: vertical;
    min-height: 150px;
}

/* Footer */
footer {
    background: #2c3e50;
    color: #fff;
    padding: 3rem 5%;
    text-align: center;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 2rem;
}

.social-links a {
    color: #fff;
    margin-left: 1rem;
    font-size: 1.5rem;
}

.copyright {
    font-size: 0.9rem;
    opacity: 0.8;
}
// Menu Burger Responsive
document.querySelector('.burger').addEventListener('click', function() {
    document.querySelector('.nav-links').classList.toggle('active');
});

// Slider automatique pour les biens (optionnel)
let currentSlide = 0;
const slides = document.querySelectorAll('.property-card');

function showSlide(n) {
    slides.forEach(slide => slide.style.display = 'none');
    currentSlide = (n + slides.length) % slides.length;
    slides[currentSlide].style.display = 'block';
}

// setInterval(() => showSlide(currentSlide + 1), 3000); // Décommentez pour un slider automatique

// Formulaire de contact
document.getElementById('contact-form').addEventListener('submit', function(e) {
    e.preventDefault();
    alert('Message envoyé ! Nous vous contacterons bientôt.');
    this.reset();
});
/* Responsive */
@media (max-width: 768px) {
    .nav-links {
        display: none;
    }

    .burger {
        display: block;
    }

    .hero-content h2 {
        font-size: 2rem;
    }
}
