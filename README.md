# sonadiemaker
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Sona Die Maker | Premium Industrial Dies</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

:root {
    --gold: #D4AF37;
    --light-gold: #F8E7A1;
    --dark-gold: #927018;
    --black: #0B0B0B;
    --dark: #171717;
    --white: #FFFFFF;
    --cream: #FAF7EF;
}

body {
    font-family: Arial, sans-serif;
    background: var(--white);
    color: #222;
    line-height: 1.7;
}

header {
    background: var(--black);
    color: var(--white);
    padding: 18px 7%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
    border-bottom: 2px solid var(--gold);
}

.logo {
    color: var(--gold);
    font-size: 25px;
    font-weight: 900;
    letter-spacing: 2px;
}

.logo small {
    display: block;
    font-size: 10px;
    letter-spacing: 4px;
    color: var(--light-gold);
}

nav {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

nav a {
    color: white;
    text-decoration: none;
    font-size: 14px;
    font-weight: bold;
}

nav a:hover {
    color: var(--gold);
}

.btn {
    display: inline-block;
    padding: 13px 25px;
    background: linear-gradient(
        135deg,
        #F8E7A1,
        #D4AF37,
        #A78018
    );
    color: #111;
    font-weight: bold;
    text-decoration: none;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: 0.3s;
}

.btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 20px #D4AF3755;
}

.hero {
    min-height: 530px;
    padding: 100px 7%;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;

    background:
        radial-gradient(
            circle at top right,
            #8A6D25 0%,
            transparent 40%
        ),
        linear-gradient(
            135deg,
            #080808,
            #211B0D,
            #080808
        );

    border-bottom: 3px solid var(--gold);
}

.hero-content {
    max-width: 850px;
}

.hero .tag {
    color: var(--gold);
    font-size: 13px;
    font-weight: bold;
    letter-spacing: 5px;
}

.hero h1 {
    color: var(--light-gold);
    font-size: clamp(38px, 7vw, 70px);
    line-height: 1.2;
    margin: 20px 0;
}

.hero p {
    max-width: 700px;
    margin: 0 auto 30px;
    color: #E0DCCF;
    font-size: 18px;
}

.hero .secondary {
    display: inline-block;
    margin: 10px;
    color: var(--gold);
    border: 1px solid var(--gold);
    padding: 11px 20px;
    text-decoration: none;
}

.highlights {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    background: var(--cream);
    padding: 30px 6%;
    text-align: center;
    gap: 20px;
}

.highlight {
    padding: 12px;
}

.highlight h3 {
    color: var(--dark-gold);
}

.highlight p {
    font-size: 13px;
    color: #666;
}

section {
    padding: 75px 8%;
}

.section-title {
    text-align: center;
    margin-bottom: 18px;
    font-size: clamp(28px, 4vw, 40px);
    color: var(--dark-gold);
}

.section-subtitle {
    text-align: center;
    max-width: 750px;
    margin: 0 auto 35px;
    color: #666;
}

.gold-line {
    width: 75px;
    height: 4px;
    background: var(--gold);
    margin: 0 auto 30px;
}

.about {
    max-width: 900px;
    margin: auto;
    text-align: center;
    font-size: 17px;
}

.services {
    background: var(--cream);
}

.cards {
    display: grid;
    grid-template-columns: repeat(
        auto-fit,
        minmax(220px, 1fr)
    );
    gap: 24px;
}

.card {
    background: white;
    padding: 30px 25px;
    border: 1px solid #E8D9A7;
    border-bottom: 4px solid var(--gold);
    border-radius: 6px;
    transition: 0.3s;
}

.card:hover {
    transform: translateY(-6px);
    box-shadow: 0 10px 25px #00000012;
}

.card .icon {
    font-size: 35px;
    margin-bottom: 12px;
}

.card h3 {
    color: var(--dark-gold);
    margin-bottom: 12px;
}

.card p {
    color: #666;
    font-size: 14px;
}

.why {
    background: var(--black);
    color: white;
}

.why .section-title {
    color: var(--light-gold);
}

.why .section-subtitle {
    color: #CCC;
}

.why-grid {
    display: grid;
    grid-template-columns: repeat(
        auto-fit,
        minmax(220px, 1fr)
    );
    gap: 25px;
    max-width: 1000px;
    margin: auto;
}

.why-box {
    border: 1px solid #D4AF3755;
    padding: 25px;
    text-align: center;
}

.why-box h3 {
    color: var(--gold);
    margin-bottom: 10px;
}

.why-box p {
    color: #DDD;
    font-size: 14px;
}

.contact {
    background: var(--cream);
}

.contact-grid {
    display: grid;
    grid-template-columns: repeat(
        auto-fit,
        minmax(280px, 1fr)
    );
    gap: 35px;
    max-width: 1000px;
    margin: auto;
}

.contact-details {
    background: var(--black);
    color: white;
    padding: 30px;
    border-top: 4px solid var(--gold);
}

.contact-details h3 {
    color: var(--gold);
    margin-bottom: 20px;
}

.contact-details p {
    margin-bottom: 16px;
    overflow-wrap: anywhere;
}

.contact-details a {
    color: var(--light-gold);
    text-decoration: none;
}

form {
    background: white;
    padding: 30px;
    border: 1px solid #E8D9A7;
    border-top: 4px solid var(--gold);
}

form h3 {
    color: var(--dark-gold);
    margin-bottom: 15px;
}

label {
    display: block;
    font-weight: bold;
    margin: 12px 0 5px;
}

input, select, textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #D5D0C2;
    border-radius: 4px;
    font-size: 15px;
    font-family: inherit;
}

textarea {
    min-height: 120px;
    resize: vertical;
}

form .btn {
    width: 100%;
    margin-top: 18px;
    font-size: 15px;
}

.form-note {
    margin-top: 12px;
    font-size: 12px;
    color: #666;
}

footer {
    background: #050505;
    color: white;
    text-align: center;
    padding: 28px 15px;
    border-top: 2px solid var(--gold);
}

footer strong {
    color: var(--gold);
}

footer p {
    font-size: 13px;
    margin: 5px;
}

@media(max-width: 650px) {
    header {
        flex-direction: column;
        text-align: center;
    }

    nav {
        justify-content: center;
        gap: 14px;
    }

    .hero {
        padding: 75px 20px;
    }

    .highlights {
        grid-template-columns: 1fr;
    }

    section {
        padding: 55px 6%;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">
        SONA DIE MAKER
        <small>PRECISION • QUALITY • TRUST</small>
    </div>

    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#why">Why Us</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<main>

<section class="hero" id="home">
    <div class="hero-content">

        <div class="tag">INDUSTRIAL DIE MANUFACTURING</div>

        <h1>Precision Dies.<br>Golden Standards.</h1>

        <p>
            Sona Die Maker specialises in embossing dies,
            cutting dies and coining dies with CNC technology.
            We welcome business enquiries from India
            and international markets.
        </p>

        <a class="btn" href="#contact">
            REQUEST AN ENQUIRY
        </a>

        <a class="secondary" href="#services">
            EXPLORE OUR SERVICES
        </a>

    </div>
</section>

<div class="highlights">

    <div class="highlight">
        <h3>Embossing Dies</h3>
        <p>Custom industrial die enquiries</p>
    </div>

    <div class="highlight">
        <h3>Cutting & Coining</h3>
        <p>Die solutions for manufacturing</p>
    </div>

    <div class="highlight">
        <h3>Global Enquiries</h3>
        <p>India and international customers</p>
    </div>

</div>

<section id="about">

    <h2 class="section-title">About Our Company</h2>

    <div class="gold-line"></div>

    <div class="about">

        <p>
            <strong>Sona Die Maker (S.D.M.)</strong> is an
            industrial die manufacturing business based in
            Chinchani, Dahanu, Palghar, Maharashtra, India.
        </p>

        <br>

        <p>
            Our work includes embossing dies, cutting dies,
            coining dies and CNC-technology-based die work.
            We welcome enquiries from companies in India
            and around the world.
        </p>

        <br>

        <p>
            Share your technical drawings, specifications
            and project requirements with us to discuss
            your industrial die needs.
        </p>

    </div>

</section>

<section class="services" id="services">

    <h2 class="section-title">Our Services</h2>

    <div class="gold-line"></div>

    <p class="section-subtitle">
        Industrial die manufacturing enquiries tailored
        to your application and specifications.
    </p>

    <div class="cards">

        <div class="card">
            <div class="icon">⚙️</div>
            <h3>Embossing Dies</h3>
            <p>
                Die solutions for embossing applications
                based on customer drawings and requirements.
            </p>
        </div>

        <div class="card">
            <div class="icon">✂️</div>
            <h3>Cutting Dies</h3>
            <p>
                Industrial cutting die enquiries for
                manufacturing applications.
            </p>
        </div>

        <div class="card">
            <div class="icon">◆</div>
            <h3>Coining Dies</h3>
            <p>
                Custom coining die requirements for
                industrial forming applications.
            </p>
        </div>

        <div class="card">
            <div class="icon">🔩</div>
            <h3>CNC Die Work</h3>
            <p>
                CNC-technology-based die work according
                to project specifications.
            </p>
        </div>

        <div class="card">
            <div class="icon">🛠️</div>
            <h3>Custom Die Enquiries</h3>
            <p>
                Contact us with your drawings, dimensions
                and project requirements.
            </p>
        </div>

        <div class="card">
            <div class="icon">🌍</div>
            <h3>International Business</h3>
            <p>
                We welcome business enquiries from India
                and international markets.
            </p>
        </div>

    </div>

</section>

<section class="why" id="why">

    <h2 class="section-title">Why Sona Die Maker?</h2>

    <div class="gold-line"></div>

    <p class="section-subtitle">
        A professional approach to industrial die enquiries.
    </p>

    <div class="why-grid">

        <div class="why-box">
            <h3>Precision Focus</h3>
            <p>
                Discuss your drawings and specifications
                for your die manufacturing requirements.
            </p>
        </div>

        <div class="why-box">
            <h3>Custom Requirements</h3>
            <p>
                Share details about your application
                to discuss suitable die solutions.
            </p>
        </div>

        <div class="why-box">
            <h3>Worldwide Enquiries</h3>
            <p>
                Contact us from India or international
                markets to start a business discussion.
            </p>
        </div>

    </div>

</section>

<section class="contact" id="contact">

    <h2 class="section-title">Contact Us</h2>

    <div class="gold-line"></div>

    <p class="section-subtitle">
        Tell us about your project. We welcome industrial
        die manufacturing and business enquiries.
    </p>

    <div class="contact-grid">

        <div class="contact-details">

            <h3>SONA DIE MAKER</h3>

            <p>
                <strong>Contact Person:</strong><br>
                Jitendra J. Dharmamer
            </p>

            <p>
                <strong>Phone / WhatsApp:</strong><br>
                <a href="https://wa.me/919168556561"
                   target="_blank" rel="noopener">
                   +91 91685 56561
                </a>
            </p>

            <p>
                <strong>Additional Phone:</strong><br>
                <a href="tel:+917020678935">
                    +91 70206 78935
                </a>
            </p>

            <p>
                <strong>Email:</strong><br>
                <a href="mailto:sonadiemaker@gmail.com">
                    sonadiemaker@gmail.com
                </a>
            </p>

            <p>
                <strong>Address:</strong><br>
                Chinchani (Mangel Aali), Tal. Dahanu,
                Dist. Palghar, Maharashtra - 401503, India
            </p>

            <p>
                <strong>Nearby Stations:</strong><br>
                Boisar / Vangaon
            </p>

            <a class="btn"
               href="https://wa.me/919168556561"
               target="_blank" rel="noopener">
               CHAT ON WHATSAPP
            </a>

        </div>

        <form id="enquiryForm">

            <h3>Business Enquiry Form</h3>

            <label for="name">Your Name *</label>
            <input id="name" name="name" required>

            <label for="company">Company Name</label>
            <input id="company" name="company">

            <label for="email">Email Address *</label>
            <input id="email" name="email"
                   type="email" required>

            <label for="country">Country</label>
            <input id="country" name="country"
                   placeholder="e.g. India">

            <label for="service">Service Required *</label>
            <select id="service" name="service" required>
                <option value="">Select Service</option>
                <option>Embossing Dies</option>
                <option>Cutting Dies</option>
                <option>Coining Dies</option>
                <option>CNC Die Work</option>
                <option>Custom Die Enquiry</option>
            </select>

            <label for="message">Project Details *</label>
            <textarea id="message" name="message"
                placeholder="Describe your requirements..."
                required></textarea>

            <button class="btn" type="submit">
                PREPARE ENQUIRY EMAIL
            </button>

            <p class="form-note">
                This form prepares an email in your email app.
                It does not send information directly to a server.
            </p>

        </form>

    </div>

</section>

</main>

<footer>
    <p><strong>SONA DIE MAKER</strong></p>
    <p>Precision Dies. Golden Standards.</p>
    <p>© <span id="year"></span> Sona Die Maker. All Rights Reserved.</p>
</footer>

<script>
document.getElementById("year").textContent =
    new Date().getFullYear();

document.getElementById("enquiryForm").addEventListener(
    "submit", function(event) {

        event.preventDefault();

        const data = new FormData(this);

        const subject = encodeURIComponent(
            "Business Enquiry - " + data.get("service")
        );

        const body = encodeURIComponent(
            "Name: " + data.get("name") + "\n" +
            "Company: " +
                (data.get("company") || "Not provided") + "\n" +
            "Email: " + data.get("email") + "\n" +
            "Country: " +
                (data.get("country") || "Not provided") + "\n" +
            "Service: " + data.get("service") + "\n\n" +
            "Project Details:\n" + data.get("message")
        );

        window.location.href =
            "mailto:sonadiemaker@gmail.com?subject=" +
            subject + "&body=" + body;
    }
);
</script>

</body>
</html>



Make a pdf
