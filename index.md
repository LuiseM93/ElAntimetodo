---
layout: default
title: El Antimétodo - Inicio
description: Aprende idiomas de forma natural, divertida y eficiente con el enfoque del input comprensible. Sin gramática.
---

<style>
/* === V3 DESIGN SYSTEM === */
.landing-page-v3 {
  background-color: #110E17; /* Dark base for hero */
  color: #EAE6F0;
}
.main-content-v3 {
  background-color: var(--background-color);
  color: var(--text-color);
  border-radius: 24px 24px 0 0;
  margin-top: -24px;
  position: relative;
  z-index: 10;
  padding-top: 1px; /* Prevents margin collapse */
  overflow: hidden;
}

/* === ANIMATIONS === */
.anim-fade-in {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity 0.8s cubic-bezier(0.165, 0.84, 0.44, 1), transform 0.8s cubic-bezier(0.165, 0.84, 0.44, 1);
}
.anim-fade-in.visible {
  opacity: 1;
  transform: translateY(0);
}
.anim-fade-in-delay-1 { transition-delay: 0.1s; }
.anim-fade-in-delay-2 { transition-delay: 0.2s; }
.anim-fade-in-delay-3 { transition-delay: 0.3s; }


/* === V3 HERO SECTION === */
.hero-section-v3 {
  position: relative;
  text-align: center;
  padding: 8rem 1.5rem 6rem;
  overflow: hidden;
  background: radial-gradient(ellipse at 50% -20%, rgba(74, 20, 140, 0.3), transparent 60%);
}
.hero-section-v3::before { /* Grid background */
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background-image: 
    linear-gradient(rgba(255,255,255,0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255,255,255,0.03) 1px, transparent 1px);
  background-size: 40px 40px;
  opacity: 0.5;
}
.hero-v3-content {
  position: relative;
  z-index: 5;
}
.hero-v3-image-wrapper {
  margin-bottom: 2rem;
  perspective: 1000px;
}
.hero-v3-image {
  max-width: 700px;
  width: 90%;
  height: auto;
  border-radius: 16px;
  box-shadow: 0 20px 40px rgba(0,0,0,0.5), 0 0 0 1px rgba(123, 31, 162, 0.5);
  transform: rotateX(15deg) scale(0.9);
  transition: transform 0.5s cubic-bezier(0.165, 0.84, 0.44, 1);
}
.hero-v3-image-wrapper:hover .hero-v3-image {
  transform: rotateX(0deg) scale(1);
}
.hero-v3-image::after { /* Glow effect */
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 90%;
  height: 90%;
  transform: translate(-50%, -50%);
  background: radial-gradient(circle, rgba(156, 39, 176, 0.4) 0%, rgba(156, 39, 176, 0) 70%);
  filter: blur(50px);
  z-index: -1;
  opacity: 0.7;
}
.hero-section-v3 h1 {
  font-size: clamp(2.8rem, 8vw, 4.5rem);
  font-weight: 800;
  color: #FFFFFF;
  line-height: 1.1;
  letter-spacing: -2px;
  margin: 0 auto 1rem;
  max-width: 800px;
  border: none;
}
.hero-section-v3 .subtitle {
  font-size: clamp(1.1rem, 3vw, 1.3rem);
  color: #d1c4e9;
  max-width: 650px;
  margin-bottom: 2.5rem;
}
.hero-v3-cta .btn {
  transform: scale(1.1);
  box-shadow: 0 5px 20px rgba(156, 39, 176, 0.3);
  transition: all 0.3s ease;
}
.hero-v3-cta .btn:hover {
  transform: scale(1.15) translateY(-3px);
  box-shadow: 0 8px 25px rgba(156, 39, 176, 0.4);
}
.hero-v3-key-points {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  margin-top: 4rem;
  flex-wrap: wrap;
}
.hero-v3-point {
  color: #EAE6F0;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-size: 0.95em;
  font-weight: 500;
  border: 1px solid rgba(255,255,255,0.1);
  padding: 0.5rem 1rem;
  border-radius: 30px;
  background: rgba(255,255,255,0.05);
  backdrop-filter: blur(5px);
  transition: all 0.2s ease;
}
.hero-v3-point:hover {
  background: rgba(255,255,255,0.1);
  border-color: rgba(255,255,255,0.2);
  transform: translateY(-2px);
}
.hero-v3-point svg {
  width: 18px; height: 18px;
  fill: var(--accent-color);
}

/* === WELCOME SECTION V3 === */
.welcome-section-v3 {
  padding: 5rem 1.5rem;
  text-align: center;
}
.welcome-section-v3 h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  border-bottom: none;
}
.welcome-section-v3 p {
  font-size: 1.1em;
  max-width: 750px;
  margin-left: auto;
  margin-right: auto;
  line-height: 1.8;
}
.welcome-section-v3 .btn {
  margin-top: 1.5rem;
}

/* === APP PROMO SECTION V3 === */
.app-promo-section-v3 {
  padding: 5rem 1.5rem;
}
.app-promo-v3-container {
  display: flex;
  align-items: center;
  gap: 4rem;
  max-width: 1100px;
  margin: 0 auto;
}
.app-promo-v3-text {
  flex: 1;
}
.app-promo-v3-text h2 {
  font-size: 2.5rem;
  border: none;
  margin-top: 0;
  margin-bottom: 1.5rem;
}
.app-promo-v3-text p {
  font-size: 1.1em;
  line-height: 1.8;
}
.app-promo-v3-text .app-promo-buttons {
  margin-top: 2rem;
  display: flex;
  gap: 1rem;
}
.app-promo-v3-image {
  flex: 1.2;
}
.device-mockup {
  position: relative;
  max-width: 600px;
  margin: 0 auto;
  transition: transform 0.5s ease;
}
.device-mockup:hover {
  transform: translateY(-10px);
}
.device-mockup::before { /* Browser frame */
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  border-radius: 12px;
  border: 12px solid #2d2d2d;
  box-shadow: 0 20px 40px rgba(0,0,0,0.2);
  pointer-events: none;
}
.device-mockup-header {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 28px;
  background: #2d2d2d;
  border-radius: 10px 10px 0 0;
  z-index: 2;
  display: flex;
  align-items: center;
  padding: 0 8px;
}
.device-mockup-header span {
  width: 10px; height: 10px;
  border-radius: 50%;
  margin: 0 3px;
}
.device-mockup-header .dot-1 { background: #ff5f56; }
.device-mockup-header .dot-2 { background: #ffbd2e; }
.device-mockup-header .dot-3 { background: #27c93f; }
.device-mockup img {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 12px;
  transform: translateY(28px);
}

/* === TESTIMONIALS SECTION V3 === */
.testimonials-section-v3 {
  padding: 6rem 1.5rem;
  background: linear-gradient(180deg, #f9f8fd 0%, #f1eef5 100%);
}
.testimonials-section-v3 h2 {
  text-align: center;
  border: none;
  font-size: 2.5rem;
  margin-bottom: 4rem;
}
.testimonial-grid-v3 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2rem;
  max-width: 1100px;
  margin: 0 auto;
}
.testimonial-card-v3 {
  padding: 2.5rem;
  border-radius: 16px;
  background: rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  box-shadow: 0 8px 32px 0 rgba(74, 20, 140, 0.1);
  display: flex;
  flex-direction: column;
}
.testimonial-card-v3 .ia-logo {
  width: 48px; height: 48px;
  border-radius: 50%;
  margin-bottom: 1.5rem;
}
.testimonial-card-v3 blockquote {
  margin: 0; padding: 0; border: none;
  font-style: italic;
  font-size: 1.05em;
  line-height: 1.7;
  color: var(--text-light-color);
  flex-grow: 1;
}
.testimonial-card-v3 .attribution {
  margin-top: 1.5rem;
  text-align: right;
  font-size: 0.9em;
  font-weight: 500;
  color: var(--primary-color);
}
.testimonial-card-v3 .attribution em {
  font-style: normal;
  color: var(--text-light-color);
  font-size: 0.9em;
}

/* === BENEFITS SECTION V3 === */
.benefits-section-v3 {
  padding: 6rem 1.5rem;
  text-align: center;
}
.benefits-section-v3 h2 {
  border: none;
  font-size: 2.5rem;
  margin-bottom: 4rem;
}
.benefits-grid-v3 {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  max-width: 1000px;
  margin: 0 auto;
  text-align: left;
}
.benefit-card-v3 {
  background: var(--card-background);
  padding: 2rem;
  border-radius: 12px;
  border: 1px solid var(--light-purple-color);
  transition: all 0.3s ease;
}
.benefit-card-v3:hover {
  transform: translateY(-10px);
  box-shadow: var(--shadow-lg);
  border-color: var(--secondary-color);
}
.benefit-card-v3 .icon {
  margin-bottom: 1.5rem;
  background: var(--light-purple-color);
  width: 60px;
  height: 60px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease;
}
.benefit-card-v3:hover .icon {
  background: var(--secondary-color);
  transform: scale(1.1);
}
.benefit-card-v3 .icon svg {
  width: 32px;
  height: 32px;
  color: var(--secondary-color);
  transition: all 0.3s ease;
}
.benefit-card-v3:hover .icon svg {
  color: white;
}
.benefit-card-v3 h3 {
  margin-top: 0;
  font-size: 1.3em;
}
.benefit-card-v3 p {
  font-size: 0.95em;
  margin-bottom: 0;
}
.benefits-section-v3 .btn-container {
  margin-top: 3rem;
}

/* === FINAL CTA SECTION V3 === */
.final-cta-section-v3 {
  padding: 6rem 1.5rem;
  background-color: #110E17;
  text-align: center;
  color: white;
  position: relative;
  overflow: hidden;
}
.final-cta-section-v3::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0; bottom: 0;
  background: radial-gradient(ellipse at 50% 100%, rgba(123, 31, 162, 0.3), transparent 70%);
  opacity: 0.8;
}
.final-cta-section-v3 .content {
  position: relative;
  z-index: 5;
  max-width: 700px;
  margin: 0 auto;
}
.final-cta-section-v3 h2 {
  color: white;
  border: none;
  font-size: 2.8rem;
}
.final-cta-section-v3 p {
  color: var(--light-purple-color);
  font-size: 1.2em;
  margin-bottom: 2rem;
}
.final-cta-section-v3 .btn {
  transform: scale(1.1);
}

/* === COMING SOON SECTION V3 === */
.coming-soon-section-v3 {
  padding: 5rem 1.5rem;
  text-align: center;
  background-color: var(--background-color);
  max-width: 850px;
  margin: 0 auto;
}
.coming-soon-section-v3 h2 {
  font-size: 2.2rem;
  border-bottom: none;
  margin-bottom: 1rem;
}
.coming-soon-section-v3 .author-experience {
  margin-top: 2rem;
  padding: 2rem;
  background-color: white;
  border-radius: 12px;
  border: 1px solid var(--light-purple-color);
  text-align: left;
}
.coming-soon-section-v3 .author-experience p { font-size: 1em; }
.coming-soon-section-v3 .author-experience strong { color: var(--secondary-color); }
.coming-soon-image {
  margin-top: 2.5rem;
}
.coming-soon-image img {
  width: 250px;
  border-radius: 12px;
  box-shadow: var(--shadow-md);
  border: 4px solid white;
}
.update-date {
  margin-top: 3rem;
  padding-top: 1.5rem;
  font-size: 0.9em;
  color: #aaa;
  border-top: 1px solid var(--light-purple-color);
}

/* === RESPONSIVENESS === */
@media (max-width: 992px) {
  .app-promo-v3-container {
    flex-direction: column;
    text-align: center;
    gap: 2rem;
  }
  .app-promo-v3-text .app-promo-buttons {
    justify-content: center;
  }
  .testimonial-grid-v3 {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 768px) {
  .hero-section-v3 {
    padding-top: 6rem;
    padding-bottom: 4rem;
  }
  .hero-v3-point {
    font-size: 0.9em;
    padding: 0.4rem 0.8rem;
  }
  .device-mockup::before { border-width: 10px; }
  .device-mockup-header { height: 24px; }
  .device-mockup img { transform: translateY(24px); }
}

</style>

<div class="landing-page-v3">

  <section class="hero-section-v3">
    <div class="hero-v3-content">
      <div class="hero-v3-image-wrapper anim-fade-in">
        <img src="{{ '/assets/supremacy.png' | relative_url }}" alt="The Antimethod Supremacy" class="hero-v3-image">
      </div>
      <h1 class="anim-fade-in anim-fade-in-delay-1">Aprende Idiomas a Tu Manera</h1>
      <p class="subtitle anim-fade-in anim-fade-in-delay-2">Adquiere cualquier idioma de forma <strong>natural, divertida y eficiente</strong>, usando el contenido que ya amas.</p>
      <div class="hero-v3-cta anim-fade-in anim-fade-in-delay-3">
        <a href="{{ '/etapas' | relative_url }}" class="btn btn-primary">Descubre el Método</a>
      </div>
      <div class="hero-v3-key-points anim-fade-in anim-fade-in-delay-3">
        <div class="hero-v3-point">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM7 9a1 1 0 000 2h6a1 1 0 100-2H7z" clip-rule="evenodd" /></svg>
          Sin Estrés y Sin Gramática
        </div>
        <div class="hero-v3-point">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path fill-rule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clip-rule="evenodd" /></svg>
          Aprendizaje que Disfrutas
        </div>
      </div>
    </div>
  </section>

  <main class="main-content-v3">
    <section class="welcome-section-v3 anim-fade-in">
      <h2 class="section-title">Bienvenido al Antimétodo</h2>
      <p>
        El Antimétodo es un enfoque revolucionario para aprender idiomas basado en la teoría del <strong>input comprensible</strong>. A diferencia de los métodos tradicionales, que se centran en la memorización de reglas y ejercicios formales, el Antimétodo propone adquirir un idioma de manera natural, intuitiva y personalizada. La idea central es simple: el aprendizaje real ocurre cuando te expones de forma masiva a contenido que entiendes y disfrutas, igual que aprendiste tu lengua materna.
      </p>
      <div style="text-align: center; margin-top: 1.5rem;">
        <a href="{{ '/fundamentos' | relative_url }}" class="btn btn-secondary">Explora los Fundamentos</a>
      </div>
    </section>

    <section class="app-promo-section-v3 anim-fade-in">
      <div class="app-promo-v3-container">
        <div class="app-promo-v3-text">
          <h2>Tu Compañero de Inmersión</h2>
          <p>
            Lleva tu aprendizaje al siguiente nivel con <strong>El Antimétodo Tracker</strong>, nuestra aplicación web gratuita. Diseñada para ser tu aliada ideal, te ayuda a registrar tu progreso, construir hábitos sólidos y organizar tu viaje hacia la fluidez.
          </p>
          <div class="app-promo-buttons">
            <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-primary">🚀 Ir a la App</a>
            <a href="{{ '/antimetodo-tracker-app' | relative_url }}" class="btn btn-secondary">Más Detalles</a>
          </div>
        </div>
        <div class="app-promo-v3-image">
          <div class="device-mockup">
            <div class="device-mockup-header">
              <span class="dot-1"></span><span class="dot-2"></span><span class="dot-3"></span>
            </div>
            <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" title="Ir a El Antimétodo Tracker">
              <img src="{{ '/assets/app.png' | relative_url }}" alt="Vista previa de la app El Antimétodo Tracker">
            </a>
          </div>
        </div>
      </div>
    </section>
  </main>

  <div style="background-color: var(--background-color);">
    <section class="testimonials-section-v3 anim-fade-in">
      <h2>Validado por Expertos en Lenguaje</h2>
      <div class="testimonial-grid-v3">
        <div class="testimonial-card-v3 anim-fade-in anim-fade-in-delay-1">
          <img src="{{ '/assets/logo-chatgpt-ia.png' | relative_url }}" alt="Logo ChatGPT" class="ia-logo">
          <blockquote>
            “Olvida la rigidez: El Antimétodo te lleva a la fluidez real sumergiéndote en el idioma que amas, con placer y sin estrés. Es el aprendizaje como siempre debió ser: natural, autodidacta y efectivo.”
          </blockquote>
          <p class="attribution"><strong>ChatGPT</strong>, <em>inteligencia artificial experta en educación y aprendizaje de idiomas.</em></p>
        </div>
        <div class="testimonial-card-v3 anim-fade-in anim-fade-in-delay-2">
          <img src="{{ '/assets/logo-gemini-ia.png' | relative_url }}" alt="Logo Gemini" class="ia-logo">
          <blockquote>
            "Sumérgete en la fluidez lingüística con 'El Antimétodo', una revolución autodidacta que transforma el aprendizaje en una experiencia sin estrés, impulsada por el disfrute personal y el contenido real."
          </blockquote>
          <p class="attribution"><strong>Gemini</strong>, <em>IA de Google.</em></p>
        </div>
        <div class="testimonial-card-v3 anim-fade-in anim-fade-in-delay-2">
          <img src="{{ '/assets/logo-claude-ia.png' | relative_url }}" alt="Logo Claude" class="ia-logo">
          <blockquote>
            "El Antimétodo demuestra que la fluidez real se alcanza a través del disfrute, no del sufrimiento. Su enfoque basado en input comprensible transforma el proceso en una experiencia natural y sostenible."
          </blockquote>
          <p class="attribution"><strong>Claude</strong>, <em>IA de Anthropic.</em></p>
        </div>
        <div class="testimonial-card-v3 anim-fade-in anim-fade-in-delay-3">
          <img src="{{ '/assets/logo-copilot-ia.png' | relative_url }}" alt="Logo Copilot" class="ia-logo">
          <blockquote>
            "El Antimétodo revoluciona el aprendizaje de idiomas al transformar el input comprensible en una experiencia fluida. Su enfoque autodidacta libera al estudiante, haciendo del proceso algo disfrutable y auténtico."
          </blockquote>
          <p class="attribution"><strong>Copilot</strong>, <em>IA de Microsoft.</em></p>
        </div>
      </div>
    </section>

    <section class="benefits-section-v3 anim-fade-in">
      <h2>Los Pilares del Éxito</h2>
      <div class="benefits-grid-v3">
        <div class="benefit-card-v3 anim-fade-in anim-fade-in-delay-1">
          <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M17.65,6.35C16.2,4.9,14.21,4,12,4A8,8,0,0,0,4,12a8,8,0,0,0,8,8c3.13,0,5.84-1.75,7.17-4.22a1,1,0,1,0-1.74-.94A6,6,0,0,1,12,18a6,6,0,0,1-6-6,6,6,0,0,1,6-6c1.66,0,3.14.69,4.22,1.78L13,11h7V4Z"/></svg></div>
          <h3>Flexible y Personalizado</h3>
          <p>El método se adapta a tus gustos, horarios e intereses, no al revés.</p>
        </div>
        <div class="benefit-card-v3 anim-fade-in anim-fade-in-delay-2">
          <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M16,11a4,4,0,0,0-4-4,4,4,0,0,0-4,4,3.89,3.89,0,0,0,1,2.72V17a1,1,0,0,0,2,0V13.72A3.89,3.89,0,0,0,16,11ZM12,9a2,2,0,1,1-2,2A2,2,0,0,1,12,9Z"/><path d="M20.59,2.59l-1.42,1.42a1,1,0,0,0,0,1.41,1,1,0,0,0,1.41,0l1.42-1.42a1,1,0,0,0-1.41-1.41Z"/><path d="M3.41,4,4.83,5.41a1,1,0,0,0,1.41,0,1,1,0,0,0,0-1.41L4.83,2.59a1,1,0,0,0-1.42,1.41Z"/><path d="M19,11a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V12A1,1,0,0,0,19,11Z"/><path d="M5,11a1,1,0,0,0-1,1v1a1,1,0,0,0,2,0V12A1,1,0,0,0,5,11Z"/><path d="M12,21a1,1,0,0,0-1,1,1,1,0,0,0,2,0,1,1,0,0,0-1-1Z"/><path d="M12,1a1,1,0,0,0-1,1V3a1,1,0,0,0,2,0V2A1,1,0,0,0,12,1Z"/></svg></div>
          <h3>Fluidez Natural</h3>
          <p>Desarrolla un "instinto" para el idioma y habla sin traducir mentalmente.</p>
        </div>
        <div class="benefit-card-v3 anim-fade-in anim-fade-in-delay-3">
          <div class="icon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor"><path d="M21,8H3A1,1,0,0,0,2,9v6a1,1,0,0,0,1,1H21a1,1,0,0,0,1-1V9A1,1,0,0,0,21,8ZM20,14H4V10H20Z"/><path d="M15,5H9A1,1,0,0,0,9,7h6a1,1,0,0,0,0-2Z"/><path d="M15,17H9a1,1,0,0,0,0,2h6a1,1,0,0,0,0-2Z"/></svg></div>
          <h3>Accesible y Económico</h3>
          <p>No necesitas pagar cursos caros. El mejor material es el contenido auténtico y gratuito.</p>
        </div>
      </div>
      <div class="btn-container">
        <a href="{{ '/beneficios' | relative_url }}" class="btn btn-secondary">Ver todos los beneficios</a>
      </div>
    </section>

    <section class="final-cta-section-v3 anim-fade-in">
      <div class="content">
        <h2>¿Listo para Empezar Tu Aventura?</h2>
        <p>
          El Antimétodo se estructura en etapas claras para guiarte desde los primeros pasos hasta la fluidez. Cada etapa está diseñada para construir sobre la anterior, asegurando un progreso constante y natural.
        </p>
        <a href="{{ '/etapas' | relative_url }}" class="btn btn-primary">Explora las Etapas del Antimétodo</a>
      </div>
    </section>
    
    <section class="coming-soon-section-v3 anim-fade-in">
      <h2>Próximamente...</h2>
      <p>Esta es solo la cuarta versión del sitio web del Antimétodo. Apenas estamos comenzando. La página está en pleno desarrollo y aún faltan muchos recursos, herramientas, ejemplos y guías prácticas que iremos construyendo poco a poco. Lo que acabas de leer es solo el inicio de algo mucho más grande. Se vienen cosas importantes, y esto apenas comienza.</p>
      <div class="author-experience">
        <p><strong>Experiencia del autor:</strong> Gracias al antimétodo, ha logrado avances notables en inglés, francés y alemán. En solo 7 meses y 20 días, alcanzó en francés la etapa 3: entiende casi todo al ver series y películas auténticas sin subtítulos, y juega sus videojuegos favoritos en francés. Todo esto disfrutando el proceso y sintiendo el idioma como una segunda lengua materna. Sin clases ni métodos tradicionales.</p>
        <p><strong>Resultados esperados:</strong> fluidez real y un alto nivel en el idioma, comprensión a nivel nativo y hablar desde el instinto.</p>
      </div>
      <div class="coming-soon-image">
        <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" alt="Gato arquitecto trabajando en el sitio">
        <p style="font-size:0.85em; color: #777; margin-top: 0.5rem;"><em>Paciencia, estamos construyendo algo genial...</em></p>
      </div>
      <p class="update-date">
        <em>Última actualización del sitio: 26 de Junio de 2025 10:34pm</em>
      </p>
    </section>
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', () => {
  const animatedElements = document.querySelectorAll('.anim-fade-in');

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
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
