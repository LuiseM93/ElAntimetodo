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
  padding: 4rem 1.5rem 5rem;
  background: linear-gradient(170deg, var(--light-purple-color) 0%, var(--background-color) 70%);
}
.app-hero .content-wrapper {
  max-width: 900px;
}
.app-hero h1 {
  font-size: clamp(2.5rem, 6vw, 3.5rem);
  font-weight: 700;
  line-height: 1.2;
  margin-bottom: 0.5rem;
  background: -webkit-linear-gradient(45deg, var(--primary-color), var(--accent-color));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  border-bottom: none;
}
.app-hero .subtitle {
  font-size: clamp(1.1rem, 3vw, 1.4rem);
  margin-bottom: 2.5rem;
  max-width: 650px;
}
.app-hero-image {
  max-width: 800px;
  width: 100%;
  margin: 1rem auto 2.5rem;
  border-radius: 12px;
  box-shadow: 0 25px 50px -12px rgba(74, 20, 140, 0.25);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.app-hero-image:hover {
  transform: translateY(-5px) scale(1.02);
  box-shadow: 0 30px 60px -15px rgba(74, 20, 140, 0.3);
}
.app-hero-cta {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
}
.app-hero-cta .btn {
  font-size: 1.1em;
  padding: 1rem 2.5rem;
}

/* How it Works Section */
.how-it-works {
  padding: 4rem 1.5rem;
  background-color: var(--background-color);
}
.how-it-works h2 {
    text-align: center;
    border-bottom: none;
    margin-bottom: 3.5rem;
    font-size: 2.2em;
}
.steps-container {
  position: relative;
  display: flex;
  justify-content: space-between;
  gap: 2rem;
  max-width: 1000px;
  margin: 0 auto;
}
.steps-container::before {
  content: '';
  position: absolute;
  top: 48px; /* Altura del ícono */
  left: 10%;
  right: 10%;
  height: 2px;
  background: repeating-linear-gradient(90deg, var(--border-purple-color), var(--border-purple-color) 6px, transparent 6px, transparent 12px);
  z-index: 0;
}
.step-card {
  position: relative;
  z-index: 1;
  text-align: center;
  background-color: var(--card-background);
  padding: 2rem 1.5rem;
  border-radius: 10px;
  box-shadow: var(--shadow-md);
  flex: 1;
  max-width: 320px;
  border-top: 4px solid var(--secondary-color);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.step-card:hover {
  transform: translateY(-8px);
  box-shadow: var(--shadow-lg);
}
.step-card .icon-wrapper {
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 96px;
  height: 96px;
  margin-bottom: 1.5rem;
  background-color: var(--light-purple-color);
  border-radius: 50%;
  border: 4px solid white;
  box-shadow: 0 0 0 4px var(--secondary-color);
}
.step-card img {
  width: 48px;
  height: 48px;
}
.step-card h3 {
  margin-top: 0;
  margin-bottom: 0.5rem;
  font-size: 1.25em;
  color: var(--primary-color);
}
.step-card p {
  font-size: 0.95em;
  color: var(--text-light-color);
  line-height: 1.6;
}

/* Features Section */
.features-section {
  padding: 5rem 1.5rem;
}
.features-section h2 {
  text-align: center;
  margin-bottom: 4rem;
  border-bottom: none;
  font-size: 2.2em;
}
.feature-item {
  display: flex;
  align-items: center;
  gap: 3rem;
  margin-bottom: 6rem;
  background-color: var(--card-background);
  padding: 3rem;
  border-radius: 16px;
  box-shadow: var(--shadow-md);
}
.feature-item:nth-child(odd) {
  flex-direction: row-reverse;
}
.feature-text {
  flex: 1;
}
.feature-text h3 {
  font-size: 2em;
  margin-top: 0;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid var(--border-purple-color);
  display: inline-block;
}
.feature-text ul {
  list-style: none;
  padding-left: 0;
  margin-top: 1.5rem;
}
.feature-text li {
  padding-left: 2em;
  position: relative;
  margin-bottom: 1rem;
  font-size: 1.05em;
}
.feature-text li::before {
  content: '';
  position: absolute;
  left: 0;
  top: 5px;
  width: 20px;
  height: 20px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' fill='%237b1fa2'%3E%3Cpath d='M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z'%3E%3C/path%3E%3C/svg%3E");
  background-size: contain;
}
.feature-image {
  flex: 1.2;
  text-align: center;
}
.feature-image img {
  max-width: 100%;
  border-radius: 10px;
  box-shadow: var(--shadow-lg);
  transition: transform 0.3s ease;
}
.feature-item:nth-child(even) .feature-image img {
    transform: rotate(2deg);
}
.feature-item:nth-child(odd) .feature-image img {
    transform: rotate(-2deg);
}
.feature-image img:hover {
    transform: rotate(0) scale(1.05);
}

/* Data Control Section */
.data-control-section {
  padding: 3rem 1.5rem;
  background-color: var(--card-background);
  border-radius: 12px;
  text-align: center;
  max-width: 800px;
  margin: 4rem auto;
  box-shadow: var(--shadow-md);
  border: 1px solid var(--border-purple-color);
}
.data-control-section h3 {
  display: inline-flex;
  align-items: center;
  gap: 0.7rem;
  margin-top: 0;
}
.data-control-section p {
  margin-bottom: 1.5rem;
}

/* Final CTA Section */
.final-cta-section {
  text-align: center;
  padding: 5rem 1.5rem;
  background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
  color: white;
  margin-left: calc(-50vw + 50%);
  margin-right: calc(-50vw + 50%);
  width: 100vw;
}
.final-cta-section h2 {
  border-bottom: none;
  color: white;
  font-size: 2.5em;
}
.final-cta-section .subtitle {
    color: var(--light-purple-color);
    opacity: 0.9;
}
.final-cta-section .btn {
    transform: scale(1.1);
    box-shadow: 0 10px 25px rgba(0,0,0,0.2);
}
.final-cta-section .btn:hover {
    transform: scale(1.15) translateY(-3px);
    box-shadow: 0 12px 30px rgba(0,0,0,0.25);
}


@media (max-width: 820px) {
  .steps-container {
    flex-direction: column;
    align-items: center;
  }
  .steps-container::before {
    top: 5%;
    bottom: 5%;
    left: 50%;
    transform: translateX(-50%);
    width: 2px;
    height: 90%;
    background: repeating-linear-gradient(180deg, var(--border-purple-color), var(--border-purple-color) 6px, transparent 6px, transparent 12px);
  }
  .feature-item, .feature-item:nth-child(odd) {
    flex-direction: column;
    gap: 2rem;
    text-align: center;
    padding: 2rem 1.5rem;
  }
  .feature-text h3 {
    display: block;
    text-align: center;
  }
  .feature-image img, 
  .feature-item:nth-child(even) .feature-image img, 
  .feature-item:nth-child(odd) .feature-image img {
      transform: rotate(0);
  }
}
</style>

<div class="app-landing-page">

  <section class="app-hero">
    <div class="content-wrapper">
      <h1>Tu Compañero Definitivo de Inmersión</h1>
      <p class="subtitle">Organiza, mide y acelera tu viaje hacia la fluidez con la herramienta gratuita creada para El Antimétodo.</p>
      <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" title="Ir a la aplicación El Antimétodo Tracker">
        <img src="{{ '/assets/app.png' | relative_url }}" alt="Interfaz de la aplicación El Antimétodo Tracker en un mockup" class="app-hero-image">
      </a>
      <div class="app-hero-cta">
        <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-primary">🚀 Ir a la App Ahora</a>
        <a href="#features" class="btn btn-secondary">Ver Funcionalidades</a>
      </div>
    </div>
  </section>

  <section class="how-it-works">
    <h2>De Cero a Hábito en 3 Pasos</h2>
    <div class="steps-container">
      <div class="step-card">
        <div class="icon-wrapper">
          <img src="{{ '/assets/rutinas-paso1-informacion.png' | relative_url }}" alt="Icono de registrar">
        </div>
        <h3>1. Registra tu Inmersión</h3>
        <p>Anota cada minuto de contenido que consumes. Ya sea viendo una serie, jugando o escuchando un podcast, cada segundo cuenta.</p>
      </div>
      <div class="step-card">
        <div class="icon-wrapper">
          <img src="{{ '/assets/rutinas-herramienta-ia-intro.png' | relative_url }}" alt="Icono de analizar">
        </div>
        <h3>2. Analiza tu Progreso</h3>
        <p>Con gráficos y estadísticas claras, visualiza tu dedicación, descubre tus patrones y mantén la motivación por las nubes.</p>
      </div>
      <div class="step-card">
        <div class="icon-wrapper">
          <img src="{{ '/assets/rutinas-principio-consistencia.png' | relative_url }}" alt="Icono de conquistar">
        </div>
        <h3>3. Conquista la Fluidez</h3>
        <p>Usa las guías integradas y las herramientas de hábitos para convertir el aprendizaje en un estilo de vida placentero y altamente efectivo.</p>
      </div>
    </div>
  </section>

  <section class="features-section" id="features">
    <div style="max-width: 1000px; margin: 0 auto;">
      <h2>Todo lo que Necesitas en un Solo Lugar</h2>

      <div class="feature-item">
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

      <div class="feature-item">
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
      
      <div class="feature-item">
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
    <h3>
      <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24" fill="currentColor" style="color:var(--primary-color);"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4zm0 10.99h7c-.53 4.12-3.28 7.79-7 8.94V12H5V6.3l7-3.11v8.8z"></path></svg>
      Tus Datos, Tu Control, Tu Privacidad
    </h3>
    <p>En El Antimétodo, creemos que eres el dueño de tu aprendizaje y de tu información. Todos tus datos se guardan exclusivamente en tu navegador. No se envían a ningún servidor. Para tu total tranquilidad, puedes exportar tu historial completo con un solo clic y guardarlo donde quieras.</p>
    <a href="{{ '/importar-tracker' | relative_url }}" class="btn btn-secondary">¿Vienes de otro tracker? Aprende a importar tus datos</a>
  </section>

  <section class="final-cta-section">
    <h2>Empieza a Aprender de Forma Inteligente. Hoy.</h2>
    <p class="subtitle">Únete a la revolución del aprendizaje de idiomas. La herramienta es gratuita, poderosa y está esperándote.</p>
    <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-primary" style="margin-top: 1rem;">🚀 Abrir El Antimétodo Tracker</a>
  </section>

</div>
