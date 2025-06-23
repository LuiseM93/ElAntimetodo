---
layout: default
title: El Antimétodo Tracker - Tu Compañero Definitivo de Inmersión
description: Descubre "El Antimétodo Tracker", la aplicación web diseñada para gestionar tu aprendizaje de idiomas, construir hábitos, acceder a guías y alcanzar la fluidez de forma natural y disfrutable.
---

<style>
.app-presentation-page .page-header {
  text-align: center;
  padding: 2rem 1rem 1.5rem 1rem; /* Menos padding inferior si la imagen va después */
}
.app-presentation-page .app-showcase-image {
  display: block;
  max-width: 750px; /* Ancho máximo para la imagen de la app */
  width: 90%; /* Responsiva */
  height: auto;
  margin: 0 auto 2.5rem auto;
  border-radius: 10px;
  box-shadow: 0 8px 25px rgba(74, 20, 140, 0.15); /* Sombra un poco más fuerte */
  border: 1px solid var(--light-purple-color);
}
.app-presentation-page .intro-section {
  font-size: 1.15em;
  text-align: center;
  color: var(--text-light-color);
  margin-bottom: 3rem;
  line-height: 1.7;
  padding: 0 1rem;
}
.app-presentation-page .intro-section strong {
    color: var(--primary-color);
}

.features-section {
  margin-bottom: 2.5rem;
}
.features-section h2.main-features-title {
    text-align: center;
    font-size: 2em;
    margin-bottom: 2.5rem;
    border-bottom: 3px solid var(--primary-color);
    display: inline-block; /* Para que el borde se ajuste al texto */
    padding-bottom: 0.5rem;
}
.features-section .center-h2-container { /* Para centrar el H2 */
    text-align: center;
}

.feature-block {
  margin-bottom: 2.5rem;
  padding: 1.8rem;
  background-color: var(--card-background);
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.07);
  border-left: 5px solid var(--secondary-color); /* Acento de color */
}
.feature-block h3 {
  color: var(--secondary-color);
  font-size: 1.5em; /* Títulos de funcionalidad más grandes */
  margin-top: 0;
  margin-bottom: 1rem;
  padding-bottom: 0.4rem;
  border-bottom: 1px dashed var(--light-purple-color);
}
.feature-block ul {
  list-style: none;
  padding-left: 0;
}
.feature-block li {
  padding-left: 1.8em;
  position: relative;
  margin-bottom: 0.8rem;
  line-height: 1.65;
}
.feature-block li::before {
  content: '✨'; /* Icono para puntos de funcionalidad */
  position: absolute;
  left: 0;
  color: var(--accent-color);
  font-size: 1em;
}
.feature-block .sub-list { /* Para listas anidadas (ej. detalles de tracker) */
    list-style-type: '▹'; /* Pequeña flecha */
    padding-left: 20px;
    margin-top: 0.5rem;
    font-size: 0.95em;
}
.feature-block .sub-list li::before {
    content: ''; /* Quitar el emoji para sub-items */
    padding-left: 0;
}
.feature-block .important-note-inline {
    display: block;
    background-color: #f0e6f6;
    padding: 0.8rem;
    border-radius: 5px;
    margin-top: 0.8rem;
    font-size: 0.95em;
    border-left: 3px solid var(--accent-color);
}

.cta-section {
  text-align: center;
  padding: 2.5rem 1rem;
  background-color: var(--light-purple-color); /* Fondo suave para el CTA */
  border-radius: 10px;
  margin-top: 3rem;
}
.cta-section .btn-app { /* Estilo específico para el botón de la app */
  font-size: 1.2em;
  padding: 1rem 2.5rem;
  background-image: linear-gradient(135deg, var(--accent-color) 0%, var(--secondary-color) 100%);
  box-shadow: 0 5px 15px rgba(123, 31, 162, 0.3);
}
.final-summary {
    margin-top: 3rem;
    padding: 1.5rem;
    background-color: var(--card-background);
    border-radius: 8px;
    border-top: 4px solid var(--primary-color);
    font-size: 1.1em;
    line-height: 1.7;
    text-align: center;
}

</style>

<main class="content-wrapper app-presentation-page">

  <div class="page-header">
    <h1>El Antimétodo Tracker</h1>
    <p class="subtitle" style="font-size: 1.3em; color: var(--secondary-color);">Tu Centro de Mando para la Fluidez</p>
  </div>

  <img src="{{ '/assets/app.png' | relative_url }}" alt="Interfaz de la aplicación El Antimétodo Tracker" class="app-showcase-image">

  <section class="intro-section">
    <p>Transforma tu aprendizaje de idiomas con <strong>El Antimétodo Tracker</strong>, la aplicación web diseñada para ser tu aliada definitiva en el camino hacia la fluidez. Olvídate de las clases aburridas y la gramática tediosa; esta herramienta te permite aplicar la filosofía del input comprensible de forma <strong>organizada, medible y motivadora</strong>.</p>
    <p>No es solo un contador de horas, es una plataforma integral para gestionar tu inmersión, construir hábitos sólidos y acceder a la guía esencial del Antimétodo, todo en un solo lugar.</p>
  </section>

  <section class="features-section">
    <div class="center-h2-container">
        <h2 class="main-features-title">¿Qué es "El Antimétodo Tracker"?<br>Tu Compañero Inteligente</h2>
    </div>
    <p style="text-align:center; max-width: 700px; margin: 0 auto 2rem auto; font-size:1.05em; color:var(--text-light-color);">Basada en los principios de adquisición natural del lenguaje, la app te ayuda a sumergirte en contenido que realmente disfrutas (series, películas, videojuegos, música) para aprender de manera intuitiva, tal como lo promueve la filosofía de <a href="{{ '/' | relative_url }}">El Antimétodo</a>.</p>

    <div class="feature-block">
      <h3>🚀 Onboarding Inteligente y Test de Ubicación</h3>
      <ul>
        <li>Comienza tu viaje con el pie derecho. La app te da una bienvenida personalizada.</li>
        <li>Te ayuda a definir tu punto de partida en El Antimétodo, sugiriendo tu etapa inicial con la ayuda de IA (si está configurada) o enlazando a nuestro <a href="{{ '/test-ubicacion' | relative_url }}">test de ubicación detallado</a> en el sitio web.</li>
        <li>Configura rápidamente tu idioma de aprendizaje y tu etapa si ya la conoces.</li>
        <li><strong>Aviso Importante:</strong> Desde el inicio se te informa que tus datos se guardan solo en tu navegador, animándote a exportarlos regularmente para tu tranquilidad.</li>
      </ul>
    </div>

    <div class="feature-block">
      <h3>📊 Tu Panel de Control (Dashboard) Motivador</h3>
      <ul>
        <li>Tu centro de operaciones visual. Observa tu progreso de un vistazo: etapa actual, cumplimiento de hábitos diarios con gráficos intuitivos, actividad reciente y consejos adaptados a ti.</li>
        <li>Mantén la motivación alta y el enfoque claro con un diseño que te inspira a seguir adelante.</li>
        <li>Selector de Idioma Activo para gestionar múltiples idiomas fácilmente.</li>
      </ul>
    </div>

    <div class="feature-block">
      <h3>⏱️ Tracker de Actividades Poderoso y Flexible</h3>
      <ul>
        <li><strong>Registra cada minuto</strong> de tu inmersión y estudio con precisión. Usa el modo manual, cronómetro o temporizador.</li>
        <li>Detalla cada sesión: idioma, categoría (Inmersión Activa/Pasiva, Estudio, Producción), sub-actividad específica (o personalizada) y notas.</li>
        <li>Edita tus registros en cualquier momento.</li>
        <li>Analiza tu dedicación con <strong>estadísticas avanzadas y gráficos detallados</strong>: tiempo total (diario, semanal, mensual), desglose por tipo de actividad y por habilidad (Listening, Reading, etc.).</li>
        <li>Establece y conquista metas de horas acumuladas (50h, 100h, 250h+) y observa tu progreso estimado.</li>
        <li>Crea y sigue tus <strong>metas personales</strong> (ej. "Ver mi primera película sin subtítulos").</li>
        <li>¡Disfruta de tu <strong>Reporte Anual estilo "Wrapped"</strong> para celebrar tus logros y compartir tu dedicación!</li>
      </ul>
    </div>
    
    <div class="feature-block">
      <h3>🛠️ Constructor de Hábitos y Rutinas Sostenibles</h3>
      <ul>
        <li>La constancia es clave, y esta app te ayuda a construirla. <strong>Define tus bloques de estudio y metas de tiempo diarias</strong>.</li>
        <li>Especifica qué categorías de actividad (Inmersión Activa, Estudio, etc.) cuentan para cada hábito.</li>
        <li>Guarda tus configuraciones como <strong>plantillas de rutinas</strong> para diferentes momentos (ej. "Rutina Intensiva de Fin de Semana", "Modo Ligero entre Semana"). Carga, renombra, actualiza o elimina tus plantillas.</li>
      </ul>
    </div>

    <div class="feature-block">
      <h3>📚 Guías y Recursos del Antimétodo Integrados</h3>
      <ul>
        <li>Accede directamente en la app a la <strong>información esencial del Antimétodo</strong>.</li>
        <li>Explicaciones detalladas de las prácticas fundamentales (Anki, minado de oraciones, tipos de inmersión).</li>
        <li>Guía completa de cada una de las 4 etapas: objetivo principal, descripción detallada, objetivos clave, consejos, desafíos y criterios para avanzar.</li>
        <li>Incluye un <strong>Explorador de Recursos</strong> curado para encontrar herramientas y contenido.</li>
      </ul>
    </div>

    <div class="feature-block">
      <h3>⚙️ Control Total sobre tu Personalización y Datos</h3>
      <ul>
        <li>Adapta la app a ti: añade tus idiomas de aprendizaje, selecciona tu idioma principal y configura preferencias de registro.</li>
        <li><strong>Tus datos son tuyos y se guardan en tu navegador.</strong></li>
        <li><strong>Exporta fácilmente toda tu información</strong> (perfil, registros, metas, rutinas) en un archivo JSON para copias de seguridad o migración.</li>
        <li>Importa datos desde un archivo JSON previamente exportado.</li>
        <li><strong>¿Vienes de otro tracker?</strong> Añade horas pasadas con la función "Importar Actividad Agregada (Bulk Import)" dentro de la app. Para una conversión más precisa de historiales detallados de otras apps, usa nuestra <a href="{{ '/importar-tracker' | relative_url }}">Guía de Importación con IA</a> disponible en este sitio web.</li>
        <li>Opción para restablecer todos tus datos y empezar de cero (con confirmación).</li>
      </ul>
    </div>

    <div class="feature-block">
      <h3>✨ Experiencia de Usuario Pulida</h3>
      <ul>
        <li>Elige entre tema Claro u Oscuro según tu preferencia.</li>
        <li>Diseño completamente responsivo para usarla cómodamente en computadoras y móviles.</li>
        <li>Una agradable pantalla de bienvenida (Splash Screen) al cargar.</li>
        <li>Totalmente gratuita y sin anuncios para un aprendizaje sin interrupciones.</li>
      </ul>
    </div>
  </section>

  <section class="cta-section">
    <h2 style="color:white; border-bottom: none;">¡Lleva tu Aprendizaje al Siguiente Nivel!</h2>
    <a href="https://luisem93.github.io/Antimetodotracker/" target="_blank" rel="noopener noreferrer" class="btn btn-app">🚀 Accede a El Antimétodo Tracker Ahora</a>
  </section>

  <section class="final-summary">
    <p>En resumen, "El Antimétodo Tracker" es mucho más que un simple contador de horas. Es una plataforma integral que te acompaña, guía, motiva y te da las herramientas para aplicar con éxito la filosofía del Antimétodo, permitiéndote aprender idiomas de una manera que se sienta efectiva y, crucialmente, que disfrutes. Te da control total sobre tus datos y te ayuda a visualizar tu progreso de formas muy detalladas y significativas.</p>
  </section>

</main>
