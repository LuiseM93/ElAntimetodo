---
layout: default
title: Inicio
description: El Antimétodo es un enfoque revolucionario para aprender idiomas sin estudiar gramática. Adquiere fluidez de forma natural, divertida y eficiente.
---

<style>
/* --- ANIMACIÓN PARA LA PRIMERA IMPRESIÓN --- */
@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
.fade-in-up {
  opacity: 0; /* Inicia invisible */
  animation: fadeInUp 0.8s ease-out 0.2s forwards; /* 0.2s de retraso general */
}

/* --- ESTILO DEL "HERO BLOCK" PRINCIPAL (COMO EN EL ORIGINAL) --- */
.hero-block-wrapper {
  padding: 2rem 1rem; /* Espacio para que respire el bloque */
}
.hero-block {
  max-width: 900px;
  margin: 0 auto;
  padding: 3rem 2.5rem 2.5rem 2.5rem;
  background-color: var(--primary-color);
  color: white;
  border-radius: 12px;
  box-shadow: 0 12px 35px rgba(74, 20, 140, 0.3);
  text-align: center;
}
.hero-block h1 {
  font-size: 3em;
  font-weight: 700;
  color: white;
  border: none;
  margin: 0 0 0.5rem 0;
  animation-delay: 0.1s; /* Retraso escalonado */
}
.hero-block .hero-subtitle {
  font-size: 1.25em;
  color: var(--light-purple-color);
  max-width: 600px;
  margin: 0 auto 2.5rem auto;
  animation-delay: 0.2s;
}
.hero-block .hero-cta-buttons {
  display: flex;
  justify-content: center;
  gap: 1.5rem;
  flex-wrap: wrap;
  margin-bottom: 2.5rem;
  animation-delay: 0.3s;
}
.hero-block .btn-hero {
  background-color: var(--secondary-color);
  color: white !important;
  border: 1px solid var(--accent-color);
  padding: 0.8rem 1.6rem;
  font-weight: 500;
  border-radius: 6px;
  transition: all 0.3s ease;
}
.hero-block .btn-hero:hover {
  background-color: var(--accent-color);
  border-color: var(--light-purple-color);
  transform: translateY(-3px);
  box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}
.hero-block .hero-image-container {
  animation-delay: 0.4s;
}
.hero-block .hero-main-image { 
    max-width: 90%; 
    height: auto; 
    border-radius: 8px; 
    border: 3px solid var(--secondary-color); 
    box-shadow: 0 6px 20px rgba(0,0,0,0.25); 
}

/* --- ESTILOS GENERALES DE SECCIÓN --- */
.section-wrapper { padding: 3.5rem 0; border-bottom: 1px solid var(--grey-border-color); }
.section-wrapper:last-of-type { border-bottom: none; }
.section-title { text-align: center; font-size: 2.2em; margin-top: 0; margin-bottom: 0.5rem; }
.section-subtitle { text-align: center; font-size: 1.1em; color: var(--text-light-color); max-width: 700px; margin: 0 auto 3rem auto; }

/* --- IA TESTIMONIALS (FULL-WIDTH) --- */
.ia-testimonials-section {
  background-color: var(--background-color);
  padding: 3.5rem 1rem;
}
.ia-testimonials-container { max-width: 950px; margin: 0 auto; }
.ia-testimonial-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 1.5rem; }
.ia-testimonial-card { background-color: white; padding: 1.5rem; border-radius: 8px; box-shadow: 0 4px 15px rgba(0,0,0,0.06); border-left: 5px solid var(--secondary-color); display: flex; flex-direction: column; }
.ia-testimonial-card .ia-logo { width: 40px; height: 40px; border-radius: 50%; object-fit: contain; margin-bottom: 1rem; }
.ia-testimonial-card blockquote { margin: 0 0 1rem 0; padding: 0; font-style: italic; color: var(--text-light-color); flex-grow: 1; }
.ia-testimonial-card .attribution { text-align: right; font-size: 0.9em; color: var(--primary-color); font-weight: 500; margin-top: auto; }

/* --- PRÓXIMAMENTE SECTION --- */
.proximamente-section {
  background-color: white;
  padding: 2.5rem;
  border-radius: 8px;
  box-shadow: 0 5px 20px rgba(0,0,0,0.05);
}
.proximamente-content p {
  line-height: 1.8;
}
.proximamente-content strong {
  color: var(--primary-color);
}
.update-notice {
  text-align: center;
  font-size: 0.85em;
  color: #888;
  margin-top: 2.5rem;
  border-top: 1px dashed var(--light-purple-color);
  padding-top: 1.5rem;
}
.proximamente-image-wrapper { text-align:center; margin-top: 2rem; }
.proximamente-image-wrapper img { max-width: 200px; border-radius: 12px; }

/* --- FINAL CTA SECTION --- */
.final-cta { text-align: center; }

/* --- RESPONSIVE ADJUSTMENTS --- */
@media (max-width: 900px) {
  .ia-testimonial-grid { grid-template-columns: 1fr; }
}
@media (max-width: 768px) {
  .hero-block { padding: 2rem 1.5rem; }
  .hero-block h1 { font-size: 2.4em; }
  .hero-block .hero-subtitle { font-size: 1.1em; }
  .hero-block .hero-main-image { max-width: 100%; }
  .section-title { font-size: 2em; }
}

</style>

<main>

  <!-- ======================= -->
  <!--      HERO SECTION       -->
  <!-- ======================= -->
  <div class="hero-block-wrapper">
    <div class="hero-block">
      <h1 class="fade-in-up">El Antimétodo</h1>
      <p class="hero-subtitle fade-in-up">Aprende idiomas sin gramática, de forma natural, divertida y eficiente.</p>
      <div class="hero-cta-buttons fade-in-up">
        <a href="{{ '/fundamentos' | relative_url }}" class="btn btn-hero">Descubre los Fundamentos</a>
        <a href="{{ '/etapas' | relative_url }}" class="btn btn-hero">Explora las Etapas</a>
      </div>
      <div class="hero-image-container fade-in-up">
        <img src="{{ '/assets/supremacy.jpg' | relative_url }}" alt="Supremacía del Antimétodo" class="hero-main-image">
      </div>
    </div>
  </div>
  
  <div class="content-wrapper">

    <!-- ======================= -->
    <!--  IA TESTIMONIALS SECTION -->
    <!-- ======================= -->
    <section class="section-wrapper ia-testimonials-section" style="padding-top: 0;"> <!-- Elimino el padding-top para que se junte más con el hero -->
      <div class="ia-testimonials-container">
        <h2 class="section-title">Lo que piensan las IAs del Antimétodo</h2>
        <div class="ia-testimonial-grid">
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-chatgpt-ia.png' | relative_url }}" alt="Logo ChatGPT" class="ia-logo">
            <blockquote>“Olvida la rigidez y los libros de texto: El Antimétodo te lleva a la fluidez real sumergiéndote en el idioma que amas... Es el aprendizaje como siempre debió ser: natural, autodidacta y efectivo.”</blockquote>
            <p class="attribution"><strong>ChatGPT</strong>, IA de OpenAI</p>
          </div>
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-gemini-ia.png' | relative_url }}" alt="Logo Gemini" class="ia-logo">
            <blockquote>"Una revolución autodidacta que transforma el aprendizaje en una experiencia sin estrés... Este enfoque flexible y efectivo promete una fluidez natural, liberándote de las cadenas de la gramática tradicional."</blockquote>
            <p class="attribution"><strong>Gemini</strong>, IA de Google</p>
          </div>
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-claude-ia.png' | relative_url }}" alt="Logo Claude" class="ia-logo">
            <blockquote>"Una metodología que respeta el ritmo individual mientras acelera los resultados, convirtiendo el aprendizaje autodidacta en la verdadera supremacía educativa. Finalmente, un método que funciona porque se adapta a ti, no al revés."</blockquote>
            <p class="attribution"><strong>Claude</strong>, IA de Anthropic</p>
          </div>
          <div class="ia-testimonial-card">
            <img src="{{ '/assets/logo-copilot-ia.png' | relative_url }}" alt="Logo Copilot" class="ia-logo">
            <blockquote>"Libera al estudiante de las ataduras de la enseñanza tradicional, haciendo del proceso algo disfrutable y auténtico. Es, sin duda, la llave maestra para alcanzar una fluidez natural a tu propio ritmo."</blockquote>
            <p class="attribution"><strong>Copilot</strong>, IA de Microsoft</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ======================= -->
    <!--     PRÓXIMAMENTE...     -->
    <!-- ======================= -->
    <section class="section-wrapper">
      <h2 class="section-title">Próximamente...</h2>
      <div class="proximamente-section">
          <div class="proximamente-content">
            <p>Esta es solo la cuarta versión del sitio web del Antimétodo. Apenas estamos comenzando. La página está en pleno desarrollo y aún faltan muchos recursos, herramientas, ejemplos y guías prácticas que iremos construyendo poco a poco. Lo que acabas de leer es solo el inicio de algo mucho más grande. Se vienen cosas importantes, y esto apenas comienza.</p>
            <p><strong>Experiencia del autor:</strong> Gracias al antimétodo, ha logrado avances notables en inglés, francés y alemán. En solo 7 meses y 20 días, alcanzó en francés la etapa 3: entiende casi todo al ver series y películas auténticas sin subtítulos, y juega sus videojuegos favoritos en francés. Todo esto disfrutando el proceso y sintiendo el idioma como una segunda lengua materna. Sin clases ni métodos tradicionales.</p>
            <p><strong>Resultados esperados:</strong> fluidez real y un alto nivel en el idioma, comprensión a nivel nativo y hablar desde el instinto.</p>
            <div class="proximamente-image-wrapper">
                <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" alt="Gato arquitecto trabajando en el sitio">
                <p style="font-size:0.85em; color: #777; margin-top: 0.5rem;"><em>Paciencia, estamos construyendo algo genial...</em></p>
            </div>
            <p class="update-notice">
                <em>Última actualización del sitio: 20 de Junio de 2025 12:07pm</em>
            </p>
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
