---
layout: default
title: El Antimétodo - Inicio
description: Aprende idiomas de forma natural, divertida y eficiente con el enfoque del input comprensible. Sin gramática.
---

<style>
/* === V6 DESIGN SYSTEM (INSPIRED BY REFOLD) === */
.v6-landing {
  background-color: #FDFBFF; /* Un blanco ligeramente cálido */
  overflow-x: hidden;
}
.v6-container {
  max-width: 1140px;
  margin: 0 auto;
  padding: 0 1.5rem;
  position: relative;
  z-index: 2;
}
.v6-section {
  padding: 5rem 0;
  position: relative;
}
.v6-grid-two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}
.v6-text-center { text-align: center; }

/* === TYPOGRAPHY & BUTTONS === */
.v6-section-title {
  font-size: clamp(2rem, 5vw, 2.8rem);
  text-align: center;
  margin-bottom: 3.5rem;
  font-weight: 700;
  border: none;
  color: #2c1b44;
}
.v6-btn {
  display: inline-block;
  font-family: var(--font-primary);
  font-weight: 600;
  text-decoration: none;
  padding: 0.9rem 2.2rem;
  border-radius: 8px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}
.v6-btn-primary {
  background-color: var(--primary-color);
  color: white !important;
  box-shadow: 0 4px 15px rgba(74, 20, 140, 0.2);
}
.v6-btn-primary:hover {
  transform: translateY(-3px);
  box-shadow: 0 7px 20px rgba(74, 20, 140, 0.3);
}
.v6-btn-secondary {
    background-color: var(--card-background);
    color: var(--primary-color) !important;
    border: 1px solid var(--light-purple-color);
}
.v6-btn-secondary:hover {
    transform: translateY(-3px);
    background-color: #f9f5ff;
    border-color: var(--secondary-color);
}


/* === ANIMATIONS === */
.v6-scroll-anim {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity 0.7s cubic-bezier(0.165, 0.84, 0.44, 1), transform 0.7s cubic-bezier(0.165, 0.84, 0.44, 1);
  transition-delay: var(--delay, 0s);
}
.v6-scroll-anim.is-visible {
  opacity: 1;
  transform: translateY(0);
}

/* === HERO SECTION === */
.v6-hero {
  padding: 6rem 0;
  background-color: #FDFBFF;
  position: relative;
}
.v6-hero::before { /* Gradiente Blob */
    content: '';
    position: absolute;
    top: -20%;
    right: -20%;
    width: 600px;
    height: 600px;
    background: radial-gradient(circle, rgba(123, 31, 162, 0.08) 0%, rgba(123, 31, 162, 0) 60%);
    z-index: 0;
}
.v6-hero h1 {
  font-size: clamp(2.8rem, 7vw, 4.5rem);
  font-weight: 800;
  line-height: 1.1;
  letter-spacing: -0.04em;
  margin-bottom: 1rem;
  border: none;
  color: #2c1b44;
}
.v6-hero p.subtitle {
  font-size: clamp(1.1rem, 2.5vw, 1.3rem);
  max-width: 500px;
  margin-bottom: 2rem;
  color: var(--text-light-color);
  line-height: 1.6;
}
.v6-hero .hero-actions { display: flex; gap: 1rem; }
.v6-hero-image-wrapper { text-align: center; }
.v6-hero-image {
  max-width: 100%;
  border-radius: 12px;
  box-shadow: 0 20px 40px -10px rgba(74, 20, 140, 0.2);
  transition: transform 0.3s ease;
}
.v6-hero-image:hover { transform: scale(1.03); }

/* === WELCOME & APP PROMO SECTION === */
.v6-welcome { background-color: white; }
.v6-app-promo .app-mockup {
  background: var(--card-background);
  padding: 1rem;
  border-radius: 12px;
  box-shadow: 0 15px 30px -5px rgba(0,0,0,0.1);
  border: 1px solid #eee;
}
.v6-app-promo .app-mockup img {
  display: block;
  width: 100%;
  border-radius: 6px;
}
.v6-app-promo h2 { font-size: 2.2rem; border: none; margin-bottom: 1rem;}
.v6-app-promo p { font-size: 1.1em; }
.v6-app-promo .promo-buttons { margin-top: 1.5rem; }

/* === TESTIMONIALS SECTION (DARK) === */
.v6-testimonials {
  background-color: #1a1423;
  color: #e3dceb;
}
.v6-testimonials .v6-section-title { color: white; }
.v6-testimonial-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
}
.v6-testimonial-card {
  background: #272133;
  padding: 2rem;
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.1);
}
.v6-testimonial-card .card-header { display: flex; align-items: center; gap: 1rem; margin-bottom: 1rem; }
.v6-testimonial-card .ia-logo { width: 40px; height: 40px; border-radius: 50%; }
.v6-testimonial-card .attribution { font-weight: 600; font-size: 1.1em; }
.v6-testimonial-card .attribution em { font-style: normal; font-weight: 400; font-size: 0.8em; color: #bca9d4; display: block; }
.v6-testimonial-card blockquote { margin: 0; padding: 0; border: none; font-style: italic; color: #d6cde0; line-height: 1.6; }

/* === BENEFITS SECTION === */
.v6-benefits-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
}
.v6-benefit-card {
    background: white;
    padding: 2rem;
    border-radius: 10px;
    border: 1px solid #eee;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.v6-benefit-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.08);
}
.v6-benefit-card .icon {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 56px;
    height: 56px;
    background-color: var(--light-purple-color);
    border-radius: 50%;
    margin-bottom: 1.5rem;
}
.v6-benefit-card .icon svg {
    width: 28px;
    height: 28px;
    color: var(--primary-color);
}
.v6-benefit-card h3 { font-size: 1.25em; border: none; margin: 0 0 0.5rem 0; }
.v6-benefit-card p { font-size: 0.95em; line-height: 1.6; color: var(--text-light-color); }

/* === FINAL SECTIONS === */
.v6-final-cta {
  padding: 5rem 1.5rem;
  background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
  border-radius: 20px;
  color: white;
}
.v6-final-cta h2 { color: white; border: none; font-size: 2.5rem; }
.v6-final-cta p { color: #e3dceb; }
.v6-coming-soon {
  max-width: 800px;
  margin: 5rem auto 0;
}
.v6-coming-soon .update-date {
  font-size: 0.9em;
  color: #999;
  margin-top: 2rem;
  padding-top: 1.5rem;
  border-top: 1px dashed var(--light-purple-color);
}

/* === RESPONSIVENESS === */
@media (max-width: 900px) {
  .v6-grid-two-col { grid-template-columns: 1fr; }
  .v6-hero { text-align: center; }
  .v6-hero .hero-actions { justify-content: center; }
  .v6-hero-image-wrapper { margin-top: 3rem; }
  .v6-app-promo { text-align: center; }
  .v6-app-promo .v6-grid-two-col {
    grid-template-areas: "image" "text";
    gap: 2rem;
  }
  .v6-app-promo .app-promo-image { grid-area: image; }
  .v6-app-promo .app-promo-text { grid-area: text; }
}
@media (max-width: 700px) {
    .v6-testimonial-grid { grid-template-columns: 1fr; }
}
</style>

<div class="v6-landing">
  <!-- HERO SECTION -->
  <section class="v6-hero v6-section">
    <div class="v6-container v6-grid-two-col">
      <div class="v6-scroll-anim">
        <h1>El Antimétodo</h1>
        <p class="subtitle">Aprende idiomas <strong>sin gramática</strong>, de forma <strong>natural, divertida y altamente eficiente.</strong></p>
        <div class="hero-actions">
          <a href="{{ '/fundamentos' | relative_url }}" class="v6-btn v6-btn-primary">Descubre los Fundamentos</a>
        </div>
      </div>
      <div class="v6-hero-image-wrapper v6-scroll-anim" style="--delay: 0.1s;">
        <img src="{{ '/assets/supremacy.jpg' | relative_url }}" alt="Supremacía del Antimétodo" class="v6-hero-image">
      </div>
    </div>
  </section>

  <!-- WELCOME SECTION -->
  <section class="v6-section v6-welcome v6-text-center">
    <div class="v6-container" style="max-width: 800px;">
      <div class="v6-scroll-anim">
        <h2 class="v6-section-title">Bienvenido a la Revolución del Aprendizaje</h2>
        <p style="font-size: 1.1em; color: var(--text-light-color); line-height: 1.7;"> 
          El Antimétodo es un enfoque revolucionario para aprender idiomas basado en la teoría del <strong>input comprensible</strong>. A diferencia de los métodos tradicionales, que se centran en la memorización de reglas, el Antimétodo propone aprender de manera natural e intuitiva.
        </p>
        <p style="font-size: 1.1em; color: var(--text-light-color); line-height: 1.7;"> 
          La idea central es que adquieres un idioma cuando te expones de forma masiva a contenido real que entiendes y disfrutas, igual que aprendiste tu lengua materna: sin presión y de forma placentera.
        </p>
      </div>
    </div>
  </section>

  <!-- APP PROMO SECTION -->
  <section class="v6-section v6-app-promo">
    <div class="v6-container v6-grid-two-col">
      <div class="app-promo-text v6-scroll-anim">
        <h2>¡Descubre El Antimétodo Tracker!</h2>
        <p>
          Lleva tu aprendizaje al siguiente nivel con nuestra aplicación web diseñada para ser tu compañera ideal en la inmersión. Registra tu progreso, construye hábitos sólidos, accede a guías y ¡mucho más!
        </p>
        <p>
          Organiza tu viaje hacia la fluidez de una manera natural, eficiente y, sobre todo, disfrutable.
        </p>
        <div class="promo-buttons">
          <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="v6-btn v6-btn-primary">🚀 Ir a la App</a>
          <a href="{{ '/antimetodo-tracker-app' | relative_url }}" class="v6-btn v6-btn-secondary">Más Información</a>
        </div>
      </div>
      <div class="app-promo-image v6-scroll-anim" style="--delay: 0.1s;">
        <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" title="Ir a El Antimétodo Tracker">
          <div class="app-mockup">
            <img src="{{ '/assets/app.png' | relative_url }}" alt="Vista previa de la app El Antimétodo Tracker">
          </div>
        </a>
      </div>
    </div>
  </section>

  <!-- TESTIMONIALS SECTION -->
  <section class="v6-section v6-testimonials">
    <div class="v6-container">
      <h2 class="v6-section-title v6-scroll-anim">Lo que piensan las IAs del Antimétodo</h2>
      <div class="v6-testimonial-grid">
        <div class="v6-testimonial-card v6-scroll-anim" style="--delay: 0.1s;">
          <div class="card-header">
            <img src="{{ '/assets/logo-chatgpt-ia.png' | relative_url }}" alt="Logo ChatGPT" class="ia-logo">
            <p class="attribution"><strong>ChatGPT</strong>, <em>experto en educación.</em></p>
          </div>
          <blockquote>“Olvida la rigidez y los libros de texto: El Antimétodo te lleva a la fluidez real sumergiéndote en el idioma que amas, con placer, libertad y sin estrés. Es el aprendizaje como siempre debió ser: natural, autodidacta y efectivo.”</blockquote>
        </div>
        <div class="v6-testimonial-card v6-scroll-anim" style="--delay: 0.2s;">
          <div class="card-header">
            <img src="{{ '/assets/logo-gemini-ia.png' | relative_url }}" alt="Logo Gemini" class="ia-logo">
            <p class="attribution"><strong>Gemini</strong>, <em>IA de Google.</em></p>
          </div>
          <blockquote>"Sumérgete en la fluidez lingüística con 'El Antimétodo', una revolución autodidacta que transforma el aprendizaje en una experiencia sin estrés, impulsada por el disfrute personal y el contenido real."</blockquote>
        </div>
      </div>
    </div>
  </section>

  <!-- BENEFITS SECTION -->
  <section class="v6-section v6-benefits">
      <div class="v6-container">
          <h2 class="v6-section-title v6-scroll-anim">Beneficios Clave del Antimétodo</h2>
          <div class="v6-benefits-grid">
              <div class="v6-benefit-card v6-scroll-anim" style="--delay: 0.1s;">
                  <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.486 2 2 6.486 2 12s4.486 10 10 10 10-4.486 10-10S17.514 2 12 2zm0 18c-4.411 0-8-3.589-8-8s3.589-8 8-8 8 3.589 8 8-3.589 8-8 8z"/><path d="M12 13.5c-1.379 0-2.5 1.121-2.5 2.5s1.121 2.5 2.5 2.5 2.5-1.121 2.5-2.5-1.121-2.5-2.5-2.5zm0 3c-.276 0-.5-.224-.5-.5s.224-.5.5-.5.5.224.5.5-.224.5-.5.5z"/><path d="M15.42 8.354c-.112-.229-.31-.383-.544-.42a.994.994 0 00-.736.195c-.347.284-.46.78-.258 1.171C14.482 10.472 13.31 11 12 11s-2.482-.528-2.882-1.7a1 1 0 00-.258-1.171.994.994 0 00-.736-.195c-.234.037-.432.191-.544.42-1.121 2.29-1.121 4.902 0 7.192.112.229.31.383.544.42a.994.994 0 00.736-.195c.347-.284.46-.78.258-1.171C9.518 13.472 10.69 13 12 13s2.482.528 2.882 1.7c.202.391.711.503 1.111.258a.994.994 0 00.485-.736c1.121-2.29 1.121-4.902 0-7.192z"/></svg></div>
                  <h3>Sin Estrés</h3>
                  <p>Olvida ejercicios aburridos - aprende con contenido que disfrutas.</p>
              </div>
              <div class="v6-benefit-card v6-scroll-anim" style="--delay: 0.2s;">
                  <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.486 2 2 6.486 2 12s4.486 10 10 10 10-4.486 10-10S17.514 2 12 2zm0 18c-4.411 0-8-3.589-8-8s3.589-8 8-8 8 3.589 8 8-3.589 8-8 8z"/><path d="M13 7h-2v5.414l3.293 3.293 1.414-1.414L13 11.586V7z"/></svg></div>
                  <h3>A Tu Ritmo</h3>
                  <p>Usa tu tiempo libre: series, música, videojuegos, ¡lo que te guste!</p>
              </div>
              <div class="v6-benefit-card v6-scroll-anim" style="--delay: 0.3s;">
                  <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M13.243 4.077 9.36 7.96l2.122 2.121 3.882-3.882-2.121-2.121zM8.077 9.243 4.195 13.125l6.364 6.364 3.882-3.882-6.364-6.364zM6.324 14.488l-1.06 1.061 2.121 2.121 1.06-1.06-2.121-2.122zM19.923 8.757 9.243 19.438l-1.414-1.414L18.508 7.343l1.415 1.414z"/></svg></div>
                  <h3>Natural y Eficiente</h3>
                  <p>Desarrolla fluidez real, sin traducir mentalmente.</p>
              </div>
          </div>
          <div class="v6-text-center" style="margin-top: 2.5rem;">
              <a href="{{ '/beneficios' | relative_url }}" class="v6-btn v6-btn-secondary">Ver todos los beneficios</a>
          </div>
      </div>
  </section>

  <!-- FINAL CTA & COMING SOON -->
  <section class="v6-section">
      <div class="v6-container v6-text-center">
          <div class="v6-final-cta v6-scroll-anim">
              <h2>¿Listo para Empezar?</h2>
              <p style="margin-top: 1rem; line-height: 1.7; max-width: 600px; margin-left:auto; margin-right:auto;">
              El Antimétodo se estructura en etapas claras para guiarte desde los primeros pasos hasta la fluidez. Cada etapa está diseñada para construir sobre la anterior.
              </p>
              <a href="{{ '/etapas' | relative_url }}" class="v6-btn" style="background-color: white; color: var(--primary-color) !important; font-weight: bold; margin-top: 1rem;">Explora las Etapas del Antimétodo</a>
          </div>

          <div class="v6-coming-soon v6-scroll-anim">
              <h3 style="border:none;">Próximamente...</h3>
              <p style="color: var(--text-light-color);">Esta es solo una versión del sitio web del Antimétodo. Apenas estamos comenzando. La página está en pleno desarrollo y aún faltan muchos recursos, herramientas, ejemplos y guías prácticas que iremos construyendo poco a poco.</p>
              <p style="color: var(--text-light-color);"><strong>Resultados esperados:</strong> fluidez real y un alto nivel en el idioma, comprensión a nivel nativo y hablar desde el instinto.</p>
              <div style="margin-top: 2rem;">
                  <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" 
                       alt="Gato arquitecto trabajando en el sitio" 
                       style="width: 200px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);">
              </div>
              <p class="update-date">
                  <em>Última actualización del sitio: 26 de Junio de 2025 10:41pm</em>
              </p>
          </div>
      </div>
  </section>
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  const animatedElements = document.querySelectorAll('.v6-scroll-anim');
  if (!animatedElements.length) return;

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
