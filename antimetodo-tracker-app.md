---
layout: default
title: El Antimétodo Tracker - Tu Compañero Definitivo de Inmersión
description: Descubre "El Antimétodo Tracker", la aplicación web diseñada para gestionar tu aprendizaje de idiomas, construir hábitos, acceder a guías y alcanzar la fluidez de forma natural y disfrutable.
---

<style>
.app-landing-page {
  /* No se necesita .content-wrapper en esta página, controlamos el ancho nosotros mismos */
}

/* Hero Section */
.app-hero {
  text-align: center;
  padding: 4rem 1.5rem 3rem;
  background: radial-gradient(circle, rgba(90, 34, 139, 0.1) 0%, rgba(249, 248, 253, 0) 70%);
}
.app-hero h1 {
  font-size: 3.2em;
  font-weight: 700;
  line-height: 1.2;
  margin-bottom: 0.5rem;
  background: -webkit-linear-gradient(45deg, var(--primary-color), var(--accent-color));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.app-hero .subtitle {
  font-size: 1.4em;
  margin-bottom: 2rem;
}
.app-hero-image {
  max-width: 800px;
  width: 100%;
  margin: 1rem auto 2.5rem;
  border-radius: 12px;
  box-shadow: var(--shadow-lg);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.app-hero-image:hover {
  transform: scale(1.02);
  box-shadow: 0 15px 35px rgba(74, 20, 140, 0.2);
}
.app-hero-cta {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
}

/* How it Works Section */
.how-it-works {
  padding: 3rem 1.5rem;
  background-color: var(--light-purple-color);
  margin-left: calc(-50vw + 50%);
  margin-right: calc(-50vw + 50%);
  width: 100vw;
}
.how-it-works h2 {
    text-align: center;
    border-bottom: none;
    margin-bottom: 2.5rem;
}
.steps-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  max-width: 1100px;
  margin: 0 auto;
}
.step-card {
  text-align: center;
  background-color: var(--card-background);
  padding: 2rem 1.5rem;
  border-radius: 10px;
  box-shadow: var(--shadow-md);
  border-top: 4px solid var(--secondary-color);
}
.step-card img {
  width: 64px;
  height: 64px;
  margin-bottom: 1rem;
}
.step-card h3 {
  margin-top: 0;
  margin-bottom: 0.5rem;
  font-size: 1.2em;
  color: var(--primary-color);
}
.step-card p {
  font-size: 0.95em;
  color: var(--text-light-color);
}


/* Features Section */
.features-section {
  padding: 4rem 1.5rem;
}
.features-section h2 {
  text-align: center;
  margin-bottom: 3rem;
  border-bottom: none;
}
.feature-row {
  display: flex;
  align-items: center;
  gap: 3rem;
  margin-bottom: 5rem;
}
.feature-row:nth-child(even) {
  flex-direction: row-reverse;
}
.feature-text {
  flex: 1;
}
.feature-text h3 {
  font-size: 1.8em;
  margin-top: 0;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid var(--border-purple-color);
  display: inline-block;
}
.feature-text ul {
  list-style: none;
  padding-left: 0;
}
.feature-text li {
  padding-left: 1.8em;
  position: relative;
  margin-bottom: 0.8rem;
}
.feature-text li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: var(--secondary-color);
  font-weight: bold;
  font-size: 1.2em;
}
.feature-image {
  flex: 1.2;
  text-align: center;
}
.feature-image img {
  max-width: 100%;
  border-radius: 10px;
  box-shadow: var(--shadow-lg);
}

/* Data Control Section */
.data-control-section {
  padding: 3rem 1.5rem;
  background-color: var(--card-background);
  border-radius: 12px;
  text-align: center;
  max-width: 800px;
  margin: 2rem auto;
  box-shadow: var(--shadow-md);
  border: 1px solid var(--border-purple-color);
}
.data-control-section h3 {
  margin-top: 0;
}
.data-control-section p {
  margin-bottom: 1.5rem;
}

/* Final CTA Section */
.final-cta-section {
  text-align: center;
  padding: 4rem 1.5rem;
}
.final-cta-section h2 {
  border-bottom: none;
}

@media (max-width: 768px) {
  .app-hero h1 { font-size: 2.5em; }
  .feature-row, .feature-row:nth-child(even) {
    flex-direction: column;
    gap: 2rem;
    text-align: center;
  }
  .feature-text h3 {
    display: block;
    text-align: center;
  }
}

</style>

<div class="app-landing-page">

  <section class="app-hero">
    <h1>Tu Compañero Definitivo de Inmersión</h1>
    <p class="subtitle">Organiza, mide y acelera tu viaje hacia la fluidez con la herramienta gratuita creada para El Antimétodo.</p>
    <img src="{{ '/assets/app.png' | relative_url }}" alt="Interfaz de la aplicación El Antimétodo Tracker en un mockup" class="app-hero-image">
    <div class="app-hero-cta">
      <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-primary" style="font-size: 1.1em; padding: 1rem 2.5rem;">🚀 Ir a la App Ahora</a>
      <a href="#features" class="btn btn-secondary" style="font-size: 1.1em; padding: 1rem 2.5rem;">Ver Funcionalidades</a>
    </div>
  </section>

  <section class="how-it-works">
    <div style="max-width: 1100px; margin: 0 auto;">
      <h2>De Cero a Hábito en 3 Pasos</h2>
      <div class="steps-container">
        <div class="step-card">
          <img src="{{ '/assets/rutinas-paso1-informacion.png' | relative_url }}" alt="Icono de registrar">
          <h3>1. Registra tu Inmersión</h3>
          <p>Anota cada minuto de contenido que consumes. Ya sea viendo una serie, jugando o escuchando un podcast, cada segundo cuenta.</p>
        </div>
        <div class="step-card">
          <img src="{{ '/assets/rutinas-herramienta-ia-intro.png' | relative_url }}" alt="Icono de analizar">
          <h3>2. Analiza tu Progreso</h3>
          <p>Con gráficos y estadísticas claras, visualiza tu dedicación, descubre tus patrones y mantén la motivación por las nubes.</p>
        </div>
        <div class="step-card">
          <img src="{{ '/assets/rutinas-principio-consistencia.png' | relative_url }}" alt="Icono de conquistar">
          <h3>3. Conquista la Fluidez</h3>
          <p>Usa las guías integradas y las herramientas de hábitos para convertir el aprendizaje en un estilo de vida placentero y altamente efectivo.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="features-section" id="features">
    <div style="max-width: 1100px; margin: 0 auto;">
      <h2>Todo lo que Necesitas en un Solo Lugar</h2>

      <div class="feature-row">
        <div class="feature-text">
          <h3>Panel de Control Inteligente</h3>
          <p>Tu centro de mando personalizado. Mira de un vistazo tu etapa actual, tus rachas de hábitos y tu actividad reciente para mantener el enfoque y la motivación siempre al máximo.</p>
          <ul>
            <li>Visualiza tu progreso diario y semanal.</li>
            <li>Recibe consejos adaptados a tu etapa.</li>
            <li>Gestiona múltiples idiomas con facilidad.</li>
          </ul>
        </div>
        <div class="feature-image">
          <img src="{{ '/assets/antimetodo-vision.jpg' | relative_url }}" alt="Dashboard de la aplicación El Antimétodo Tracker">
        </div>
      </div>

      <div class="feature-row">
        <div class="feature-text">
          <h3>Tracker de Actividades Flexible</h3>
          <p>Registra tu tiempo con la precisión que necesitas. Usa el cronómetro, el temporizador o añade entradas manualmente. Cada minuto de tu esfuerzo merece ser contado.</p>
          <ul>
            <li>Clasifica tus actividades por categoría y habilidad.</li>
            <li>Analiza tu dedicación con estadísticas avanzadas.</li>
            <li>Establece y persigue metas de horas acumuladas.</li>
          </ul>
        </div>
        <div class="feature-image">
          <img src="{{ '/assets/rutinas-planificacion-general.png' | relative_url }}" alt="Gráficos de seguimiento de tiempo en la app">
        </div>
      </div>
      
      <div class="feature-row">
        <div class="feature-text">
          <h3>Constructor de Hábitos Sostenibles</h3>
          <p>La constancia es el superpoder del aprendizaje. Define tus metas diarias y semanales, crea rutinas personalizadas y haz que la inmersión sea una parte natural de tu día a día.</p>
          <ul>
            <li>Establece objetivos de tiempo flexibles.</li>
            <li>Guarda plantillas de rutinas para diferentes días.</li>
            <li>Observa cómo tus hábitos se consolidan con el tiempo.</li>
          </ul>
        </div>
        <div class="feature-image">
          <img src="{{ '/assets/rutina-inmersion-extrema.png' | relative_url }}" alt="Calendario de hábitos en la app">
        </div>
      </div>
    </div>
  </section>

  <section class="data-control-section">
    <h3>Tus Datos, Tu Control, Tu Privacidad</h3>
    <p>En El Antimétodo, creemos que eres el dueño de tu aprendizaje y de tu información. Todos tus datos se guardan exclusivamente en tu navegador. No se envían a ningún servidor. Para tu total tranquilidad, puedes exportar tu historial completo con un solo clic y guardarlo donde quieras.</p>
    <a href="{{ '/importar-tracker' | relative_url }}" class="btn btn-secondary">¿Vienes de otro tracker? Aprende a importar tus datos</a>
  </section>

  <section class="final-cta-section">
    <h2>Empieza a Aprender de Forma Inteligente. Hoy.</h2>
    <p class="subtitle">Únete a la revolución del aprendizaje de idiomas. La herramienta es gratuita, poderosa y está esperándote.</p>
    <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-primary" style="font-size: 1.2em; padding: 1.2rem 3rem;">🚀 Abrir El Antimétodo Tracker</a>
  </section>

</div>
