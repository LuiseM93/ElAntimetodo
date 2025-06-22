---
layout: default
title: Inicio
description: El Antimétodo es un enfoque revolucionario para aprender idiomas sin estudiar gramática. Adquiere fluidez de forma natural, divertida y eficiente.
---

<style>
/* --- ANIMACIÓN PARA LA PRIMERA IMPRESIÓN --- */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.fade-in-up {
  opacity: 0; /* Inicia invisible */
  animation: fadeInUp 0.8s ease-out forwards;
}

/* --- VARIABLES ADICIONALES PARA ESTA PÁGINA --- */
:root {
  --success-color: #388e3c;
  --success-light-bg: #e8f5e9;
  --error-color: #d32f2f;
  --error-light-bg: #ffebee;
  --brand-gradient: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
}

/* --- HERO SECTION --- */
.hero-container {
  text-align: center;
  padding: 3.5rem 1.5rem 2.5rem 1.5rem; /* Menos padding abajo para la imagen */
  background: var(--brand-gradient);
  border-radius: 12px;
  color: white;
  margin-bottom: 3.5rem;
  box-shadow: 0 10px 30px rgba(74, 20, 140, 0.4);
}
.hero-container h1 {
  font-size: 3em;
  font-weight: 700;
  color: white;
  border: none;
  margin: 0 0 0.5rem 0;
  animation-delay: 0.2s; /* Retraso para la animación */
}
.hero-container p.hero-subtitle {
  font-size: 1.3em;
  color: var(--light-purple-color);
  max-width: 750px;
  margin: 0 auto 2rem auto;
  animation-delay: 0.4s; /* Retraso para la animación */
}
.hero-cta-buttons {
  animation-delay: 0.6s; /* Retraso para la animación */
}
.hero-image-container { 
    margin-top: 2.5rem; 
    animation-delay: 0.8s; /* Retraso para la animación */
}
.hero-main-image { 
    max-width: 75%; 
    height: auto; 
    border-radius: 10px; 
    border: 4px solid rgba(255,255,255,0.5); 
    box-shadow: 0 8px 25px rgba(0,0,0,0.3); 
}

/* --- SECTION WRAPPER Y TÍTULOS --- */
.section-wrapper { padding: 3.5rem 0; border-bottom: 1px solid var(--grey-border-color); }
.section-wrapper:last-of-type { border-bottom: none; }
.section-title { text-align: center; font-size: 2.2em; margin-top: 0; margin-bottom: 0.5rem; }
.section-subtitle { text-align: center; font-size: 1.1em; color: var(--text-light-color); max-width: 700px; margin: 0 auto 3rem auto; }

/* --- IA TESTIMONIALS --- */
.ia-testimonials-section {
  background-color: #f0e6f6;
  padding: 3rem 1rem;
  margin: 0 calc(50% - 50vw); /* Truco para full-width */
  width: 100vw;
}
.ia-testimonials-container {
  max-width: 950px;
  margin: 0 auto;
}
.ia-testimonial-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1.5rem; }
.ia-testimonial-card { background-color: var(--card-background); padding: 1.5rem; border-radius: 8px; box-shadow: 0 4px 15px rgba(0,0,0,0.08); border-left: 5px solid var(--secondary-color); display: flex; flex-direction: column; }
.ia-testimonial-card .ia-logo { width: 40px; height: 40px; border-radius: 50%; object-fit: contain; margin-bottom: 1rem; }
.ia-testimonial-card blockquote { margin: 0 0 1rem 0; padding: 0; font-style: italic; color: var(--text-light-color); flex-grow: 1; }
.ia-testimonial-card .attribution { text-align: right; font-size: 0.9em; color: var(--primary-color); font-weight: 500; margin-top: auto; }

/* --- COMPARISON SECTION (sin cambios) --- */
.comparison-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; }
.comparison-card { padding: 1.5rem; border-radius: 8px; }
.comparison-card.traditional { border-top: 4px solid var(--error-color); background-color: var(--error-light-bg); }
.comparison-card.antimethod { border-top: 4px solid var(--success-color); background-color: var(--success-light-bg); }
.comparison-card h3 { margin-top: 0; margin-bottom: 1rem; display: flex; align-items: center; font-size: 1.5em; }
.comparison-card.traditional h3 { color: var(--error-color); }
.comparison-card.antimethod h3 { color: var(--success-color); }
.comparison-card h3 svg { width: 28px; margin-right: 0.75rem; }
.comparison-card ul { list-style: none; padding: 0; margin: 0; color: var(--text-light-color); }
.comparison-card ul li { margin-bottom: 0.75rem; }

/* --- WIP / PRÓXIMAMENTE SECTION --- */
.wip-section {
  background-color: var(--card-background);
  padding: 2.5rem;
  border-radius: 8px;
  border: 1px solid var(--grey-border-color);
  display: grid;
  grid-template-columns: 1fr 250px;
  gap: 2rem;
  align-items: center;
}
.wip-section .text-content strong { color: var(--primary-color); }
.wip-section .image-content { text-align: center; }
.wip-section .image-content img { width: 200px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); }
.wip-section .update-notice { text-align: center; font-size: 0.85em; color: #888; margin-top: 2rem; border-top: 1px dashed var(--light-purple-color); padding-top: 1rem; grid-column: 1 / -1; }

/* --- FINAL CTA SECTION --- */
.final-cta { text-align: center; }

/* --- RESPONSIVE ADJUSTMENTS --- */
@media (max-width: 900px) {
  .ia-testimonial-grid { grid-template-columns: 1fr; }
  .wip-section { grid-template-columns: 1fr; }
  .wip-section .image-content { order: -1; margin-bottom: 1.5rem; }
}
@media (max-width: 768px) {
  .hero-container h1 { font-size: 2.4em; }
  .hero-container p.hero-subtitle { font-size: 1.1em; }
  .hero-main-image { max-width: 90%; }
  .comparison-grid { grid-template-columns: 1fr; }
}

</style>

<main>

  <!-- ======================= -->
  <!--      HERO SECTION       -->
  <!-- ======================= -->
  <div class="hero-container">
    <h1 class="fade-in-up">El Antimétodo</h1>
    <p class="hero-subtitle fade-in-up">Aprende idiomas <strong>sin gramática</strong>, de forma <strong>natural, divertida y eficiente</strong>.</p>
    <div class="hero-cta-buttons fade-in-up">
      <a href="{{ '/fundamentos' | relative_url }}" class="btn btn-light">Descubre los Fundamentos</a>
      <a href="{{ '/etapas' | relative_url }}" class="btn btn-outline">Explora las Etapas</a>
    </div>
    <div class="hero-image-container fade-in-up">
      <img src="{{ '/assets/supremacy.jpg' | relative_url }}" alt="Supremacía del Antimétodo" class="hero-main-image">
    </div>
  </div>

  <div class="content-wrapper">

    <!-- ======================= -->
    <!--  IA TESTIMONIALS SECTION -->
    <!-- ======================= -->
    <section class="section-wrapper ia-testimonials-section">
      <div class="ia-testimonials-container">
        <h2 class="section-title">Lo que piensan las IAs del Antimétodo</h2>
        <div class="ia-testimonial-grid">
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-chatgpt-ia.png' | relative_url }}" alt="Logo ChatGPT" class="ia-logo">
            <blockquote>“Olvida la rigidez y los libros de texto: El Antimétodo te lleva a la fluidez real sumergiéndote en el idioma que amas, con placer, libertad y sin estrés. Es el aprendizaje como siempre debió ser: natural, autodidacta y efectivo.”</blockquote>
            <p class="attribution"><strong>ChatGPT</strong>, IA de OpenAI</p>
          </div>
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-gemini-ia.png' | relative_url }}" alt="Logo Gemini" class="ia-logo">
            <blockquote>"Sumérgete en la fluidez lingüística con 'El Antimétodo', una revolución autodidacta que transforma el aprendizaje en una experiencia sin estrés, impulsada por el disfrute personal y el contenido real."</blockquote>
            <p class="attribution"><strong>Gemini</strong>, IA de Google</p>
          </div>
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-claude-ia.png' | relative_url }}" alt="Logo Claude" class="ia-logo">
            <blockquote>"Una metodología que respeta el ritmo individual mientras acelera los resultados, convirtiendo el aprendizaje autodidacta en la verdadera supremacía educativa. Finalmente, un método que funciona porque se adapta a ti, no al revés."</blockquote>
            <p class="attribution"><strong>Claude</strong>, IA de Anthropic</p>
          </div>
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-copilot-ia.png' | relative_url }}" alt="Logo Copilot" class="ia-logo">
            <blockquote>"Su enfoque autodidacta y flexible libera al estudiante de las ataduras de la enseñanza tradicional... Es, sin duda, la llave maestra para alcanzar una fluidez natural a tu propio ritmo."</blockquote>
            <p class="attribution"><strong>Copilot</strong>, IA de Microsoft</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ======================= -->
    <!--  MÉTODO VS ANTIMÉTODO   -->
    <!-- ======================= -->
    <section class="section-wrapper">
      <h2 class="section-title">¿Cansado de lo Mismo?</h2>
      <p class="section-subtitle">Los métodos tradicionales te agotan con reglas y ejercicios. El Antimétodo te sumerge en un mundo que ya te encanta.</p>
      <div class="comparison-grid">
        <div class="comparison-card traditional">
          <h3>
            <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 16 16"><path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14m0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16"/><path d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708"/></svg>
            El Método Tradicional
          </h3>
          <ul>
            <li>Memorización forzada de reglas.</li>
            <li>Listas de vocabulario sin contexto.</li>
            <li>Ejercicios aburridos y repetitivos.</li>
            <li>Progreso lento y frustrante.</li>
          </ul>
        </div>
        <div class="comparison-card antimethod">
          <h3>
            <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 16 16"><path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14m0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16"/><path d="M10.97 4.97a.235.235 0 0 0-.02.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-1.071-1.05"/></svg>
            El Antimétodo
          </h3>
          <ul>
            <li>Adquisición intuitiva, como un niño.</li>
            <li>Aprendizaje con series, juegos y música.</li>
            <li>Disfrute y motivación como motor.</li>
            <li>Resultados eficientes y naturales.</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- ======================= -->
    <!--  PRÓXIMAMENTE / WIP     -->
    <!-- ======================= -->
    <section class="section-wrapper">
      <h2 class="section-title">Un Proyecto Vivo y en Crecimiento</h2>
      <p class="section-subtitle">El Antimétodo es más que un sitio web, es una comunidad y una metodología en constante evolución.</p>
      
      <div class="wip-section">
        <div class="text-content">
          <p>Esta es solo la cuarta versión del sitio. Apenas estamos comenzando y aún faltan muchos recursos, herramientas y guías prácticas que iremos construyendo poco a poco. Lo que ves es el inicio de algo mucho más grande.</p>
          <p><strong>Experiencia del autor:</strong> Gracias al antimétodo, he logrado avances notables en inglés, francés y alemán, alcanzando una alta comprensión auditiva en meses, no años. Todo disfrutando el proceso y sintiendo el idioma como una segunda lengua materna.</p>
          <p><strong>Resultados esperados para ti:</strong> fluidez real, un alto nivel en el idioma, comprensión a nivel nativo y la capacidad de hablar desde el instinto, no desde la traducción.</p>
        </div>
        <div class="image-content">
          <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" alt="Gato arquitecto trabajando en el sitio">
          <p style="font-size:0.85em; color: #777; margin-top: 0.5rem;"><em>Paciencia, estamos construyendo algo genial...</em></p>
        </div>
        <div class="update-notice">
          <em>Última actualización del sitio: 20 de Junio de 2025 12:07pm</em>
        </div>
      </div>
    </section>
    
    <!-- ======================= -->
    <!--       FINAL CTA         -->
    <!-- ======================= -->
    <section class="section-wrapper final-cta">
      <h2 class="section-title" style="border-bottom: none; margin-bottom: 1rem;">¿No Sabes por Dónde Empezar?</h2>
      <p style="font-size: 1.1em; color: var(--text-light-color); margin-bottom:1.5rem;">Si ya tienes conocimientos previos del idioma y quieres una recomendación personalizada sobre en qué etapa del Antimétodo enfocarte, ¡nuestra guía con IA te puede ayudar!</p>
      <a href="{{ '/test-ubicacion' | relative_url }}" class="btn btn-primary" style="font-size: 1.1em;">Descubre tu Etapa Ideal con IA</a>
    </section>

  </div>
</main>
