<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PaySecure</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <nav class="navbar">
        <div class="container">
            <div class="logo">💳 PaySecure</div>
            <ul class="nav-links">
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#paiement">Paiement</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <section id="accueil" class="hero">
        <div class="container">
            <h1>Bienvenue sur PaySecure</h1>
            <p>La plateforme de paiement la plus sécurisée et fiable</p>
            <button class="btn btn-primary" onclick="document.getElementById('paiement').scrollIntoView()">Commencer</button>
        </div>
    </section>

    <section id="services" class="services">
        <div class="container">
            <h2>Nos Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">🔒</div>
                    <h3>Sécurisé</h3>
                    <p>Chiffrement SSL 256-bit et protection PCI-DSS</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">⚡</div>
                    <h3>Rapide</h3>
                    <p>Traitement instantané des paiements</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🌍</div>
                    <h3>International</h3>
                    <p>Accepte plus de 150 devises</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📱</div>
                    <h3>Mobile</h3>
                    <p>Compatible avec tous les appareils</p>
                </div>
            </div>
        </div>
    </section>

    <section id="paiement" class="payment-section">
        <div class="container">
            <h2>Effectuer un Paiement</h2>
            <form class="payment-form" id="paymentForm">
                <div class="form-row">
                    <div class="form-group">
                        <label>Nom Complet</label>
                        <input type="text" id="fullName" placeholder="Jean Dupont" required>
                    </div>
                    <div class="form-group">
                        <label>Email</label>
                        <input type="email" id="email" placeholder="jean@exemple.com" required>
                    </div>
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label>Montant (EUR)</label>
                        <input type="number" id="amount" placeholder="100.00" min="0.01" step="0.01" required>
                    </div>
                    <div class="form-group">
                        <label>Description</label>
                        <input type="text" id="description" placeholder="Description du paiement" required>
                    </div>
                </div>

                <div class="form-group">
                    <label>Numéro de Carte</label>
                    <input type="text" id="cardNumber" placeholder="1234 5678 9012 3456" maxlength="19" required>
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label>Date d'Expiration</label>
                        <input type="text" id="expiryDate" placeholder="MM/YY" maxlength="5" required>
                    </div>
                    <div class="form-group">
                        <label>CVV</label>
                        <input type="text" id="cvv" placeholder="123" maxlength="4" required>
                    </div>
                </div>

                <button type="submit" class="btn btn-success">Payer Sécurisé</button>
                <p class="security-notice">🔒 Paiement sécurisé avec SSL 256-bit</p>
            </form>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2>Nous Contacter</h2>
            <p>Des questions ? Notre équipe est disponible 24/7</p>
            <div class="contact-info">
                <div><strong>Email:</strong> support@paysecure.com</div>
                <div><strong>Téléphone:</strong> +33 1 23 45 67 89</div>
                <div><strong>Adresse:</strong> 123 Avenue de Paris, 75000 Paris</div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2026 PaySecure. Tous droits réservés.</p>
            <div class="footer-links">
                <a href="#">Mentions légales</a>
                <a href="#">Politique de confidentialité</a>
                <a href="#">Conditions d'utilisation</a>
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
