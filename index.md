---
layout: default
title: El Antimétodo - Inicio
description: Aprende idiomas de forma natural, divertida y eficiente con el enfoque del input comprensible. Sin gramática.
---

<style>
/* === V4 DESIGN SYSTEM === */
.landing-page-v4 {
  overflow-x: hidden;
}
.main-content-v4 {
  background-color: var(--background-color);
  color: var(--text-color);
}
.v4-section {
  padding: 6rem 1.5rem;
  position: relative;
}
.v4-container {
  max-width: 1100px;
  margin: 0 auto;
  position: relative;
  z-index: 2;
}
.v4-section-title {
  font-size: clamp(2rem, 5vw, 2.8rem);
  text-align: center;
  margin-bottom: 4rem;
  font-weight: 700;
  border: none;
}

/* === ANIMATIONS === */
.scroll-anim {
  opacity: 0;
  transform: translateY(40px);
  transition: opacity 0.8s cubic-bezier(0.165, 0.84, 0.44, 1), transform 0.8s cubic-bezier(0.165, 0.84, 0.44, 1);
}
.scroll-anim.is-visible {
  opacity: 1;
  transform: translateY(0);
}
@for $i from 1 through 5 {
  .scroll-anim-delay-#{$i} {
    transition-delay: #{$i * 0.1}s;
  }
}

/* === HERO SECTION V4 === */
.hero-v4 {
  padding: 8rem 1.5rem 10rem;
  text-align: center;
  background: linear-gradient(180deg, #f5f3f9 0%, var(--background-color) 100%);
}
.hero-v4 h1 {
  font-size: clamp(3rem, 9vw, 6rem);
  font-weight: 800;
  line-height: 1.05;
  letter-spacing: -0.04em;
  margin: 0 auto 1.5rem;
  border: none;
  color: #1a0a2e;
}
.hero-v4 .subtitle {
  font-size: clamp(1.1rem, 3vw, 1.4rem);
  max-width: 700px;
  margin-bottom: 2.5rem;
  color: var(--text-light-color);
}
.hero-v4-image-container {
  margin-top: 4rem;
}
.hero-v4-image {
  max-width: 750px;
  width: 95%;
  border-radius: 12px;
  box-shadow: 0 25px 50px -12px rgba(74, 20, 140, 0.25);
  transition: transform 0.8s cubic-bezier(0.165, 0.84, 0.44, 1);
}
.hero-v4-image-container:hover .hero-v4-image {
  transform: scale(1.05);
}

/* === SVG DIVIDER === */
.wave-divider {
  position: absolute;
  bottom: -1px;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
}
.wave-divider svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 120px;
}
.wave-divider .shape-fill {
  fill: var(--background-color);
}
.wave-divider.top-divider {
    top: -1px;
    bottom: auto;
    transform: rotate(0);
}

/* === APP PROMO SECTION V4 === */
.app-promo-v4 {
  background-color: var(--background-color);
  padding-top: 8rem;
}
.app-promo-v4-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}
.app-promo-v4-text h2 {
  font-size: 2.5rem;
  margin-bottom: 1.5rem;
  border: none;
}
.app-promo-v4-text p {
  font-size: 1.1em;
  line-height: 1.8;
}
.app-promo-v4-text .app-promo-buttons {
  margin-top: 2rem;
  display: flex;
  gap: 1rem;
}
.app-promo-v4-image .device-mockup {
  max-width: 500px;
  transform: rotate(3deg);
  transition: transform 0.3s ease;
}
.app-promo-v4-image .device-mockup:hover {
  transform: rotate(0deg) scale(1.03);
}
.device-mockup {
  border-radius: 12px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.2);
}
.device-mockup img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 12px;
}

/* === TESTIMONIALS SECTION V4 === */
.testimonials-v4 {
  background-color: #110E17;
  color: #EAE6F0;
}
.testimonials-v4 .v4-section-title {
  color: white;
}
.testimonial-grid-v4 {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2.5rem;
}
.testimonial-card-v4 {
  background: #1c1627;
  padding: 2.5rem;
  border-radius: 12px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  display: flex;
  flex-direction: column;
  position: relative;
  overflow: hidden;
}
.testimonial-card-v4::before { /* Quote character */
  content: '“';
  position: absolute;
  top: -10px;
  left: 15px;
  font-size: 8rem;
  color: rgba(255, 255, 255, 0.05);
  font-family: serif;
  line-height: 1;
  z-index: 1;
}
.testimonial-card-v4 .ia-logo {
  width: 48px; height: 48px;
  border-radius: 50%;
  margin-bottom: 1.5rem;
  position: relative;
  z-index: 2;
}
.testimonial-card-v4 blockquote {
  margin: 0; padding: 0; border: none;
  font-style: italic;
  font-size: 1.05em;
  line-height: 1.7;
  color: #c5b9d6;
  flex-grow: 1;
  position: relative;
  z-index: 2;
}
.testimonial-card-v4 .attribution {
  margin-top: 1.5rem;
  font-size: 0.9em;
  font-weight: 500;
  color: white;
  position: relative;
  z-index: 2;
}
.testimonial-card-v4 .attribution em {
  font-style: normal;
  color: #c5b9d6;
  font-size: 0.9em;
  display: block;
}

/* === BENEFITS SECTION V4 === */
.benefits-v4-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}
.benefit-card-v4 {
  background-color: white;
  padding: 2.5rem 2rem;
  border-radius: 12px;
  border: 1px solid var(--light-purple-color);
  position: relative;
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.benefit-card-v4:hover {
  transform: translateY(-8px);
  box-shadow: var(--shadow-lg);
}
.benefit-card-v4::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: var(--secondary-color);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.4s cubic-bezier(0.19, 1, 0.22, 1);
}
.benefit-card-v4:hover::after {
  transform: scaleX(1);
}
.benefit-card-v4 .icon {
  margin-bottom: 1.5rem;
}
.benefit-card-v4 .icon svg {
  width: 36px;
  height: 36px;
  color: var(--secondary-color);
}
.benefit-card-v4 h3 {
  font-size: 1.4em;
  margin-top: 0;
  margin-bottom: 0.5rem;
}
.benefit-card-v4 p {
  font-size: 0.95em;
  line-height: 1.6;
  margin-bottom: 0;
}
.benefits-v4 .btn-container {
  margin-top: 3rem;
  text-align: center;
}

/* === FINAL SECTIONS V4 === */
.final-cta-v4 {
  text-align: center;
}
.final-cta-v4 h2 {
  font-size: 2.8rem;
  border: none;
}
.final-cta-v4 p {
  color: var(--text-light-color);
  font-size: 1.2em;
  margin-bottom: 2rem;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}
.coming-soon-v4 {
  max-width: 800px;
  margin: 6rem auto 0;
  padding: 2.5rem;
  background-color: white;
  border-radius: 16px;
  text-align: center;
  border: 1px solid var(--light-purple-color);
}
.coming-soon-v4 h3 {
  border-bottom: 1px solid var(--border-purple-color);
  display: inline-block;
  padding-bottom: 0.5rem;
  margin-top: 0;
}
.coming-soon-v4 .update-date {
  margin-top: 2rem;
  padding-top: 1rem;
  font-size: 0.9em;
  color: #aaa;
  border-top: 1px dashed var(--light-purple-color);
}
.coming-soon-v4 .gato-img {
    width: 150px;
    margin-top: 1rem;
    border-radius: 50%;
    border: 4px solid var(--light-purple-color);
}


/* === RESPONSIVENESS === */
@media (max-width: 900px) {
  .app-promo-v4-grid {
    grid-template-columns: 1fr;
    text-align: center;
  }
  .app-promo-v4-grid .app-promo-buttons {
    justify-content: center;
  }
  .app-promo-v4-image {
    order: -1;
  }
}
@media (max-width: 768px) {
  .v4-section { padding: 4rem 1.5rem; }
  .hero-v4 { padding: 5rem 1.5rem 6rem; }
}

</style>

<div class="landing-page-v4">

  <section class="hero-v4">
    <div class="v4-container scroll-anim">
      <h1>Aprende idiomas sin esfuerzo.</h1>
      <p class="subtitle">El Antimétodo es el camino natural hacia la fluidez a través del contenido que ya amas. Olvida las reglas, empieza a disfrutar.</p>
      <a href="{{ '/etapas' | relative_url }}" class="btn btn-primary">Descubre cómo funciona</a>
      <div class="hero-v4-image-container">
        <img src="{{ '/assets/supremacy.jpg' | relative_url }}" alt="The Antimethod Supremacy" class="hero-v4-image">
      </div>
    </div>
  </section>

  <main class="main-content-v4">
    <section class="v4-section app-promo-v4">
        <div class="wave-divider top-divider">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M985.66,92.83C906.67,72,823.78,31,743.84,14.19c-82.26-17.34-168.06-16.33-250.45.39-57.84,11.73-114,31.07-172,41.86A600.21,600.21,0,0,1,0,27.35V120H1200V95.8C1132.19,118.92,1055.71,111.31,985.66,92.83Z" class="shape-fill"></path>
            </svg>
        </div>
      <div class="v4-container app-promo-v4-grid scroll-anim">
        <div class="app-promo-v4-text">
          <h2>Tu compañero de inmersión</h2>
          <p>Lleva tu aprendizaje al siguiente nivel con <strong>El Antimétodo Tracker</strong>, nuestra aplicación web gratuita. Diseñada para ser tu aliada ideal, te ayuda a registrar tu progreso, construir hábitos sólidos y organizar tu viaje hacia la fluidez.</p>
          <div class="app-promo-buttons">
            <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-primary">🚀 Ir a la App</a>
            <a href="{{ '/antimetodo-tracker-app' | relative_url }}" class="btn btn-secondary">Más Detalles</a>
          </div>
        </div>
        <div class="app-promo-v4-image">
          <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" title="Ir a El Antimétodo Tracker">
            <div class="device-mockup">
                <img src="{{ '/assets/app.png' | relative_url }}" alt="Vista previa de la app El Antimétodo Tracker">
            </div>
          </a>
        </div>
      </div>
    </section>

    <section class="v4-section testimonials-v4">
      <div class="v4-container">
        <h2 class="v4-section-title scroll-anim">Validado por Expertos en Lenguaje</h2>
        <div class="testimonial-grid-v4">
          <div class="testimonial-card-v4 scroll-anim scroll-anim-delay-1">
            <img src="{{ '/assets/logo-chatgpt-ia.png' | relative_url }}" alt="Logo ChatGPT" class="ia-logo">
            <blockquote>“Olvida la rigidez: El Antimétodo te lleva a la fluidez real sumergiéndote en el idioma que amas, con placer y sin estrés. Es el aprendizaje como siempre debió ser: natural, autodidacta y efectivo.”</blockquote>
            <p class="attribution"><strong>ChatGPT</strong> <em>Experto en educación y aprendizaje de idiomas.</em></p>
          </div>
          <div class="testimonial-card-v4 scroll-anim scroll-anim-delay-2">
            <img src="{{ '/assets/logo-gemini-ia.png' | relative_url }}" alt="Logo Gemini" class="ia-logo">
            <blockquote>"Sumérgete en la fluidez lingüística con 'El Antimétodo', una revolución autodidacta que transforma el aprendizaje en una experiencia sin estrés, impulsada por el disfrute personal y el contenido real."</blockquote>
            <p class="attribution"><strong>Gemini</strong> <em>IA de Google.</em></p>
          </div>
        </div>
      </div>
    </section>

    <section class="v4-section benefits-v4">
      <div class="v4-container">
        <h2 class="v4-section-title scroll-anim">Los Pilares del Éxito</h2>
        <div class="benefits-v4-grid">
          <div class="benefit-card-v4 scroll-anim scroll-anim-delay-1">
            <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M17.65,6.35C16.2,4.9,14.21,4,12,4A8,8,0,0,0,4,12a8,8,0,0,0,8,8c3.13,0,5.84-1.75,7.17-4.22a1,1,0,1,0-1.74-.94A6,6,0,0,1,12,18a6,6,0,0,1-6-6,6,6,0,0,1,6-6c1.66,0,3.14.69,4.22,1.78L13,11h7V4Z"/></svg></div>
            <h3>Flexible y Personalizado</h3>
            <p>El método se adapta a tus gustos, horarios e intereses, no al revés.</p>
          </div>
          <div class="benefit-card-v4 scroll-anim scroll-anim-delay-2">
            <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M16,11a4,4,0,0,0-4-4,4,4,0,0,0-4,4,3.89,3.89,0,0,0,1,2.72V17a1,1,0,0,0,2,0V13.72A3.89,3.89,0,0,0,16,11ZM12,9a2,2,0,1,1-2,2A2,2,0,0,1,12,9Z"/><path d="M20.59,2.59l-1.42,1.42a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l1.42-1.42a1,1,0,0,0-1.41-1.41Z"/><path d="M3.41,4,4.83,5.41a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41L4.83,2.59a1,1,0,0,0-1.42,1.41Z"/><path d="M19,11a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V12A1,1,0,0,0,19,11Z"/><path d="M5,11a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V12A1,1,0,0,0,5,11Z"/><path d="M12,21a1,1,0,0,0-1,1,1,1,0,0,0,2,0,1,1,0,0,0-1-1Z"/><path d="M12,1a1,1,0,0,0-1,1V3a1,1,0,0,0,2,0V2A1,1,0,0,0,12,1Z"/></svg></div>
            <h3>Fluidez Natural</h3>
            <p>Desarrolla un "instinto" para el idioma y habla sin traducir mentalmente.</p>
          </div>
          <div class="benefit-card-v4 scroll-anim scroll-anim-delay-3">
            <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M21,8H3A1,1,0,0,0,2,9v6a1,1,0,0,0,1,1H21a1,1,0,0,0,1-1V9A1,1,0,0,0,21,8ZM20,14H4V10H20Z"/><path d="M15,5H9A1,1,0,0,0,9,7h6a1,1,0,0,0,0-2Z"/><path d="M15,17H9a1,1,0,0,0,0,2h6a1,1,0,0,0,0-2Z"/></svg></div>
            <h3>Accesible y Económico</h3>
            <p>No necesitas pagar cursos caros. El mejor material es el contenido auténtico y gratuito.</p>
          </div>
        </div>
        <div class="btn-container">
          <a href="{{ '/beneficios' | relative_url }}" class="btn btn-secondary">Ver todos los beneficios</a>
        </div>
      </div>
    </section>

    <section class="v4-section final-cta-v4">
      <div class="v4-container">
        <div class="scroll-anim">
          <h2>¿Listo para Empezar Tu Aventura?</h2>
          <p>El Antimétodo se estructura en etapas claras para guiarte desde los primeros pasos hasta la fluidez. Cada etapa está diseñada para construir sobre la anterior, asegurando un progreso constante y natural.</p>
          <a href="{{ '/etapas' | relative_url }}" class="btn btn-primary">Explora las Etapas del Antimétodo</a>
        </div>
        
        <div class="coming-soon-v4 scroll-anim">
          <h3>Próximamente...</h3>
          <p>Esta es solo una de las versiones del sitio web del Antimétodo. Apenas estamos comenzando y la página está en pleno desarrollo. ¡Se vienen cosas importantes!</p>
          <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" alt="Gato arquitecto trabajando en el sitio" class="gato-img">
          <p class="update-date">
            <em>Última actualización del sitio: 26 de Junio de 2025 10:41pm</em>
          </p>
        </div>
      </div>
    </section>

  </main>
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  const animatedElements = document.querySelectorAll('.scroll-anim');

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('is-visible');
        observer.unobserve(entry.target);
      }
    });
  }, {
    threshold: 0.1
  });

  animatedElements.forEach(el => {
    observer.observe(el);
  });
});
</script>
