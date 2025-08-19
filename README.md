<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Funeraria Aires de Paz</title>
  <style>
    body {
      font-family: 'Lato', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    h1, h2, h3 {
      font-family: 'Playfair Display', serif;
      color: #2b3a67;
    }

    header {
      background: linear-gradient(to right, #2b3a67, #1a2238);
      color: #fff;
      text-align: center;
      padding: 3rem 1rem;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 0.5rem;
    }

    nav {
      margin-top: 1rem;
    }

    nav a {
      margin: 0 1rem;
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #c0a060;
    }

    section {
      max-width: 1000px;
      margin: auto;
      padding: 2rem 1rem;
      opacity: 0;
      transform: translateY(30px);
      transition: all 0.7s ease;
    }

    section.show {
      opacity: 1;
      transform: translateY(0);
    }

    .section-title {
      text-align: center;
      margin-bottom: 2rem;
      font-size: 2rem;
      color: #c0a060;
    }

    /* -------- SERVICIOS (Acordeón) -------- */
    .accordion {
      background: #fff;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.08);
      margin-bottom: 1rem;
      overflow: hidden;
    }

    .accordion-header {
      background: #2b3a67;
      color: #fff;
      padding: 1rem;
      cursor: pointer;
      font-weight: bold;
    }

    .accordion-content {
      max-height: 0;
      overflow: hidden;
      background: #fff;
      padding: 0 1rem;
      transition: max-height 0.4s ease, padding 0.4s ease;
    }

    .accordion.active .accordion-content {
      max-height: 300px;
      padding: 1rem;
    }

    /* -------- MAPA -------- */
    .map-container {
      text-align: center;
      margin-top: 2rem;
    }

    iframe {
      border: none;
      border-radius: 12px;
      width: 100%;
      height: 400px;
    }

    /* -------- FORMULARIO -------- */
    form {
      background: #fff;
      padding: 2rem;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.08);
    }

    input, textarea {
      width: 100%;
      padding: 0.8rem;
      margin: 0.5rem 0;
      border: 1px solid #ccc;
      border-radius: 8px;
    }

    button {
      background: #2b3a67;
      color: #fff;
      border: none;
      padding: 0.8rem 1.5rem;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s;
    }

    button:hover {
      background: #1a2238;
    }

    /* -------- WHATSAPP FLOAT -------- */
    .whatsapp-float {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25D366;
      color: #fff;
      border-radius: 50%;
      padding: 15px;
      font-size: 24px;
      text-decoration: none;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      transition: transform 0.3s;
      z-index: 2000;
    }

    .whatsapp-float:hover {
      transform: scale(1.1);
    }

    /* -------- FOOTER -------- */
    footer {
      background: #2b3a67;
      color: #fff;
      text-align: center;
      padding: 2rem 1rem;
      margin-top: 3rem;
    }

    footer a {
      color: #c0a060;
      text-decoration: none;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <!-- ENCABEZADO -->
  <header>
    <h1>Funeraria Aires de Paz</h1>
    <p>Serenidad, respeto y dignidad para su familia</p>
    <nav>
      <a href="#historia">Historia</a>
      <a href="#ubicacion">Ubicación</a>
      <a href="#servicios">Servicios</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <!-- HISTORIA -->
  <section id="historia">
    <h2 class="section-title">Nuestra Historia</h2>
    <p><strong>Aires de Paz</strong> nació en el año 2022 en Guayaquil, gracias a la visión de su propietario <strong>Sr. Jaime Sánchez Farías</strong>. La funeraria fue creada con el propósito de brindar un servicio humano, digno y solidario a las familias, incluyendo traslados sin costo adicional a los lugares de origen.</p>
  </section>

  <!-- UBICACIÓN -->
  <section id="ubicacion">
    <h2 class="section-title">Ubicación</h2>
    <p>Nos encontramos en <strong>Colinas de la Alborada Norte</strong>, Guayaquil – Ecuador.</p>
    <div class="map-container">
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!..."></iframe>
    </div>
  </section>

  <!-- SERVICIOS (Acordeón Web 2.0) -->
  <section id="servicios">
    <h2 class="section-title">Nuestros Servicios</h2>

    <div class="accordion">
      <div class="accordion-header">Servicio Funeral Tradicional</div>
      <div class="accordion-content">
        <ul>
          <li>Cofre Mortuorio Tradicional.</li>
          <li>Transporte y útiles de velación.</li>
          <li>Retiro del fallecido.</li>
          <li>Formolización 24h.</li>
          <li>2 arreglos florales.</li>
        </ul>
      </div>
    </div>

    <div class="accordion">
      <div class="accordion-header">Servicio Funeral Clásico</div>
      <div class="accordion-content">
        <ul>
          <li>Cofre Metálico.</li>
          <li>Transporte y útiles de velación.</li>
          <li>Retiro del fallecido.</li>
          <li>Formolización 24h.</li>
          <li>3 arreglos florales.</li>
        </ul>
      </div>
    </div>

    <div class="accordion">
      <div class="accordion-header">Servicio Funeral Moderno</div>
      <div class="accordion-content">
        <ul>
          <li>Cofre de madera tallada.</li>
          <li>Transporte y útiles de velación.</li>
          <li>Retiro del fallecido.</li>
          <li>Formolización 24h.</li>
          <li>4 arreglos florales.</li>
        </ul>
      </div>
    </div>

    <div class="accordion">
      <div class="accordion-header">Servicio Funeral Exclusivo</div>
      <div class="accordion-content">
        <ul>
          <li>Cofre Exclusivo.</li>
          <li>Traslado + maquillaje.</li>
          <li>Formolización 24h.</li>
          <li>Movilización familiar.</li>
          <li>Arreglos florales y servicio de mesa.</li>
          <li>Servicio de Réquiem.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- CONTACTO -->
  <section id="contacto">
    <h2 class="section-title">Contáctenos</h2>
    <form onsubmit="enviarMensaje(event)">
      <input type="text" id="nombre" placeholder="Nombre completo" required>
      <input type="email" id="email" placeholder="Correo electrónico" required>
      <textarea id="mensaje" rows="4" placeholder="Escriba su mensaje..." required></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <!-- FOOTER -->
  <footer>
    <p>📍 Dirección: Colinas de la Alborada Norte, Guayaquil – Ecuador</p>
    <p>☎️ Teléfono: +593 999 123 456 | 📧 Email: <a href="mailto:contacto@airesdepaz.com">contacto@airesdepaz.com</a></p>
    <p>&copy; 2025 Funeraria Aires de Paz – Todos los derechos reservados</p>
  </footer>

  <!-- BOTÓN WHATSAPP -->
  <a href="https://wa.me/593999123456" class="whatsapp-float">💬</a>

  <script>
    // Animaciones de scroll
    const sections = document.querySelectorAll("section");
    window.addEventListener("scroll", () => {
      sections.forEach(sec => {
        const top = sec.getBoundingClientRect().top;
        if (top < window.innerHeight - 100) {
          sec.classList.add("show");
        }
      });
    });

    // Acordeón interactivo
    const accordions = document.querySelectorAll(".accordion");
    accordions.forEach(acc => {
      acc.querySelector(".accordion-header").addEventListener("click", () => {
        acc.classList.toggle("active");
      });
    });

    // Simulación de envío de formulario
    function enviarMensaje(e) {
      e.preventDefault();
      alert("Gracias por contactarnos. Nos comunicaremos pronto.");
      e.target.reset();
    }
  </script>

</body>
</html>
