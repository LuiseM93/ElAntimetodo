---
layout: default
title: Recursos y Herramientas - El Antimétodo
description: Herramientas, aplicaciones, mazos de Anki y fuentes de input para aprender idiomas con El Antimétodo, organizados por etapa y utilidad.
---

<style>
.resource-section {
  margin-bottom: 2.5rem;
  padding: 1.5rem;
  background-color: var(--card-background);
  border-radius: 8px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.05);
}
.resource-section h2 {
  margin-top: 0;
  border-bottom: 2px solid var(--light-purple-color);
  padding-bottom: 0.5rem;
  margin-bottom: 1.5rem;
}
.resource-section h3 {
  color: var(--secondary-color);
  margin-top: 1.8rem; 
  margin-bottom: 1rem;
  border-bottom: 1px dashed var(--light-purple-color);
  padding-bottom: 0.4rem; 
  font-size: 1.3em; 
}
.resource-section h4 {
    color: var(--primary-color);
    margin-top: 1.2rem; 
    margin-bottom: 0.5rem;
    font-size: 1.15em; 
    /* Para alinear con logo si se usa */
    /* display: flex; */
    /* align-items: center; */
}
.resource-item {
  margin-bottom: 1.2rem; 
}
.resource-item ul {
  list-style-type: disc;
  padding-left: 25px; 
  margin-top: 0.5rem;
}
.resource-item li {
  margin-bottom: 0.4rem; 
  display: flex; /* Para alinear logo dentro del li con el texto */
  align-items: center;
}
.price-tag, .free-tag, .warning-tag, .note-tag { 
  display: inline-block;
  padding: 0.2em 0.6em; 
  font-size: 0.8em;
  border-radius: 4px; 
  margin-left: 8px; /* Aumentado margen para tags */
  font-weight: bold;
  vertical-align: middle; 
}
.price-tag { background-color: #ffe0b2; color: #e65100; border: 1px solid #e65100; }
.free-tag { background-color: #c8e6c9; color: #2e7d32; border: 1px solid #2e7d32; }
.warning-tag strong { color: #ef5350; } 
.note-tag { background-color: #e3f2fd; color: #0d47a1; border: 1px solid #0d47a1; }

.resource-item p.description {
    font-size: 0.95em;
    color: var(--text-light-color); 
    margin-top: 0.3rem;
    margin-bottom: 0.6rem;
    line-height: 1.6;
}
.resource-item .platforms {
    font-size: 0.85em;
    color: #777;
    margin-top: 0.2rem;
}

/* Estilos para Logos en listas y títulos */
.resource-logo {
  width: 22px; /* Tamaño estándar para logos en listas */
  height: 22px;
  margin-right: 8px;
  object-fit: contain; 
  vertical-align: middle; /* Mejor alineación vertical con texto */
  border-radius: 3px;
}
.resource-category > h3 > .resource-logo { /* Para logos en títulos H3 */
    width: 26px;
    height: 26px;
    margin-right: 10px;
}

</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Recursos y Herramientas</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">Tu arsenal para conquistar cualquier idioma con El Antimétodo.</p>
  </section>

  <!-- SECCIÓN IMPORTANTE: SEGUIMIENTO DE TIEMPO -->
  <section class="resource-section">
    <h2>⭐ Seguimiento de Tiempo (¡Esencial!)</h2>
    <div class="resource-item">
      <h4><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo">Refold Tracker</h4>
      <p class="description">Aplicación esencial para registrar tu tiempo de inmersión y estudio, ayudándote a medir tu progreso y mantener la motivación.</p>
      <ul>
        <li><a href="https://www.notion.so/refold/Descargar-la-App-de-Refold-ES-16d4fa7e6fbd4a909068c310a36df275" target="_blank" rel="noopener noreferrer">Información y Descarga (Notion de Refold)</a></li>
        <li><a href="https://play.google.com/store/apps/details?id=com.refoldla.habitsmobile&hl=en" target="_blank" rel="noopener noreferrer">Descargar en Play Store (Android)</a></li>
      </ul>
    </div>
    <div class="resource-item">
      <h4>Alternativas a Refold Tracker:</h4>
      <p class="description"><span class="note-tag">Recomendamos Refold Tracker</span> para El Antimétodo, pero estas son otras opciones:</p>
      <ul>
        <li><a href="https://toggl.com/track/" target="_blank" rel="noopener noreferrer">Toggl Track</a></li>
        <li><a href="https://polylogger.com/auth/login" target="_blank" rel="noopener noreferrer">Polylogger</a></li>
      </ul>
    </div>
  </section>

  <!-- ETAPA 1 -->
  <section class="resource-section">
    <h2>Etapa 1: Preparación Previa</h2>
    
    <div class="resource-category">
      <h3><img src="{{ '/assets/logo-anki.png' | relative_url }}" alt="Logo Anki" class="resource-logo">Anki (Sistema de Repetición Espaciada)</h3>
      <p class="description">Herramienta fundamental para memorizar vocabulario y frases de manera eficiente.</p>
      <div class="resource-item">
        <h4>Descargar Anki:</h4>
        <ul>
          <li><a href="https://apps.ankiweb.net" target="_blank" rel="noopener noreferrer">PC / Mac / Linux (Web Oficial)</a></li>
          <li><a href="https://play.google.com/store/apps/details?id=com.ichi2.anki" target="_blank" rel="noopener noreferrer">AnkiDroid (Android)</a> <span class="free-tag">Gratis</span></li>
          <li><a href="https://apps.apple.com/us/app/ankimobile-flashcards/id373493387" target="_blank" rel="noopener noreferrer">AnkiMobile (iOS)</a> <span class="warning-tag">⚠️</span> <span class="price-tag">De pago ($24.99 USD aprox.)</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Mazos Recomendados para Anki:</h4>
        <ul>
          <li><a href="https://refold.la/es/category/decks/" target="_blank" rel="noopener noreferrer"><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo">Mazos de Refold</a> <span class="price-tag">De pago ($20 USD aprox.)</span> - <em>Excelente calidad.</em></li>
          <li><a href="https://refold.link/community-deck-spanish" target="_blank" rel="noopener noreferrer"><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo">Mazo 1000 Palabras Inglés (Comunidad Refold)</a> <span class="free-tag">Gratis</span> <span class="warning-tag">⚠️</span> - <em>Basado en español. Revisar calidad.</em></li>
          <li><a href="https://ankiweb.net/shared/info/539815993" target="_blank" rel="noopener noreferrer">Mazo 1000 Palabras (Inglés a Francés)</a> <span class="free-tag">Gratis</span> <span class="warning-tag">⚠️</span> - <em>Comunidad.</em></li>
          <li><a href="https://ankiweb.net/shared/info/1366502789" target="_blank" rel="noopener noreferrer">Mazo Fonética del Francés</a> <span class="free-tag">Gratis</span></li>
        </ul>
      </div>
    </div>

    <div class="resource-category">
      <h3><img src="{{ '/assets/logo-busuu.png' | relative_url }}" alt="Logo Busuu" class="resource-logo">Plataformas de Aprendizaje Inicial</h3>
      <div class="resource-item">
        <h4>Busuu <span class="note-tag">Recomendada</span></h4>
        <p class="description">Para construir una base inicial en el idioma. Ofrece lecciones estructuradas.</p>
        <ul>
          <li><a href="https://www.busuu.com/es/hp" target="_blank" rel="noopener noreferrer">Sitio Web de Busuu</a></li>
        </ul>
        <p class="platforms">Disponible en Play Store y App Store.</p>
      </div>
    </div>
  </section>

  <!-- ETAPA 2 -->
  <section class="resource-section">
    <h2>Etapa 2: Inmersión Total en el Idioma</h2>
    <div class="resource-category">
      <h3>Asistentes de Lectura, Video y Contenido</h3>
      <div class="resource-item">
        <h4><img src="{{ '/assets/logo-language-reactor.png' | relative_url }}" alt="Logo Language Reactor" class="resource-logo">Language Reactor</h4>
        <p class="description">Extensión para navegadores (Netflix, YouTube, etc.).</p>
        <ul>
          <li><a href="https://www.languagereactor.com" target="_blank" rel="noopener noreferrer">Sitio Web de Language Reactor</a></li>
          <li>Tutorial por Mr. Salas: <a href="https://www.youtube.com/watch?v=99JDJeCovHs" target="_blank" rel="noopener noreferrer">Ver video</a></li>
        </ul>
      </div>
       <div class="resource-item">
        <h4><img src="{{ '/assets/logo-lingq.png' | relative_url }}" alt="Logo LingQ" class="resource-logo">LingQ</h4>
        <p class="description">Plataforma de lectura y audio sincronizado.</p>
        <ul>
            <li><a href="https://www.lingq.com/en/" target="_blank" rel="noopener noreferrer">Sitio Web de LingQ</a> <span class="price-tag">De pago (opción gratuita limitada)</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Readlang</h4>
        <p class="description">Alternativa a LingQ para lectura. <span class="warning-tag">⚠️</span> <span class="note-tag">En exploración.</span></p>
        <ul>
            <li><a href="https://readlang.com" target="_blank" rel="noopener noreferrer">Sitio Web de Readlang</a> <span class="price-tag">De pago ($6 USD/mes, opción gratuita limitada)</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Lute (Alternativa Gratuita)</h4>
        <p class="description">Software de código abierto para lectura intensiva.</p>
        <ul>
            <li>Tutorial de Lute por Refold: <a href="https://www.youtube.com/watch?v=mN6kUfrKpvk" target="_blank" rel="noopener noreferrer">Ver video</a></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Voracious</h4>
        <p class="description">Reproductor de video local para aprendizaje. <span class="warning-tag">⚠️</span> <span class="note-tag">En exploración.</span></p>
        <ul>
            <li><a href="https://voracious.app" target="_blank" rel="noopener noreferrer">Sitio Web de Voracious</a></li>
        </ul>
      </div>
    </div>

    <div class="resource-category">
        <h3>Plataformas de Streaming</h3>
        <p class="description">Para encontrar series, películas y documentales.</p>
        <ul>
            <li><img src="{{ '/assets/logo-netflix.png' | relative_url }}" alt="Logo Netflix" class="resource-logo"><a href="https://www.netflix.com" target="_blank" rel="noopener noreferrer">Netflix</a></li>
            <li><a href="https://www.primevideo.com" target="_blank" rel="noopener noreferrer">Prime Video</a></li>
            <li><a href="https://www.disneyplus.com" target="_blank" rel="noopener noreferrer">Disney Plus</a></li>
            <li><img src="{{ '/assets/logo-youtube.png' | relative_url }}" alt="Logo YouTube" class="resource-logo"><a href="https://www.youtube.com" target="_blank" rel="noopener noreferrer">YouTube</a> <span class="free-tag">Gratis</span></li>
            <li><a href="https://www.france.tv" target="_blank" rel="noopener noreferrer">France.tv</a> <span class="free-tag">Gratis</span> - <em>(puede requerir VPN).</em></li>
        </ul>
    </div>
     <div class="resource-category">
        <h3>VPN (Para Acceder a Contenido Geobloqueado)</h3>
        <div class="resource-item">
            <h4><img src="{{ '/assets/logo-urban-vpn.png' | relative_url }}" alt="Logo Urban VPN" class="resource-logo">Urban VPN</h4>
            <p class="description">Cambia tu ubicación virtual.</p>
            <ul>
                <li><a href="https://www.urban-vpn.com" target="_blank" rel="noopener noreferrer">Sitio Web de Urban VPN</a> <span class="free-tag">Gratis (con opciones de pago)</span></li>
            </ul>
            <p class="platforms">Disponible en Play Store y App Store.</p>
        </div>
    </div>
    <div class="resource-category">
        <h3>Consejos de Inmersión Adicionales</h3>
        <ul>
            <li>Crea una cuenta de YouTube nueva para tu idioma meta.</li>
            <li>Cambia el idioma de Netflix, teléfono y otros dispositivos.</li>
        </ul>
    </div>
  </section>

  <!-- ETAPA 3 -->
  <section class="resource-section">
    <h2>Etapa 3: Free Flow Listening y Minado de Oraciones</h2>
    <div class="resource-category">
      <h3>Técnicas y Herramientas de Estudio Avanzado</h3>
      <div class="resource-item">
        <h4>Intensive Listening</h4>
        <ul>
          <li>Tutorial de Refold: <a href="https://www.youtube.com/watch?v=o8857j-RwhA" target="_blank" rel="noopener noreferrer">Ver video</a></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Minado de Oraciones (Sentence Mining)</h4>
        <ul>
          <li>Tutorial manual: <a href="https://www.youtube.com/watch?v=0TKEytorfdY" target="_blank" rel="noopener noreferrer">Ver video</a></li>
          <li><strong>Importante:</strong> Mina solo oraciones i+1. Traduce la oración completa.</li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Herramientas para Minado Asistido/Automático:</h4>
        <ul>
            <li><a href="https://migaku.com" target="_blank" rel="noopener noreferrer">Migaku</a> <span class="price-tag">De pago</span></li>
            <li><a href="https://yomitan.wiki" target="_blank" rel="noopener noreferrer">Yomitan (Extensión)</a> <span class="free-tag">Gratis</span> <span class="warning-tag">⚠️</span> - <em>Para Antimétodo, mejor minar oraciones completas.</em></li>
        </ul>
      </div>
    </div>
  </section>
  
  <!-- INMERSIÓN PASIVA -->
  <section class="resource-section">
    <h2>Inmersión Pasiva (Recomendada desde Etapa 2)</h2>
    <div class="resource-item">
      <h4>Plataformas de Podcasts:</h4>
      <ul>
        <li><img src="{{ '/assets/logo-spotify.png' | relative_url }}" alt="Logo Spotify" class="resource-logo"><a href="https://www.spotify.com" target="_blank" rel="noopener noreferrer">Spotify</a></li>
        <li><a href="https://play.google.com/store/apps/details?id=com.bambuna.podcastaddict&hl=en" target="_blank" rel="noopener noreferrer">Podcast Addict (Android)</a> <span class="free-tag">Gratis</span></li>
        <li>Apple Podcasts (iOS) <span class="free-tag">Gratis</span></li>
      </ul>
    </div>
    <div class="resource-item">
        <h4>Radio Online:</h4>
        <ul>
            <li><a href="https://www.radiofrance.fr" target="_blank" rel="noopener noreferrer">Radio France</a> <span class="free-tag">Gratis</span></li>
            <li class="platforms" style="list-style-type:none; margin-left:-20px;"><em>(Aplicaciones disponibles en Play Store y App Store)</em></li>
        </ul>
    </div>
  </section>

  <!-- ETAPA 4 -->
  <section class="resource-section">
    <h2>Etapa 4: Producción del Idioma</h2>
    <div class="resource-category">
      <h3>Práctica de Conversación (Escrita y Oral)</h3>
       <div class="resource-item">
        <h4>Inteligencia Artificial (IA) para Conversar:</h4>
        <ul>
          <li><img src="{{ '/assets/logo-chatgpt.png' | relative_url }}" alt="Logo ChatGPT" class="resource-logo"><a href="https://chatgpt.com" target="_blank" rel="noopener noreferrer">ChatGPT</a></li>
          <li><a href="https://character.ai" target="_blank" rel="noopener noreferrer">Character.ai</a></li>
          <li><a href="https://www.issen.com/es/" target="_blank" rel="noopener noreferrer">Issen (Tutor IA)</a> <span class="price-tag">De pago</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Intercambio de Idiomas con Nativos <span class="free-tag">Gratis</span></h4>
        <ul>
          <li><img src="{{ '/assets/logo-tandem.png' | relative_url }}" alt="Logo Tandem" class="resource-logo"><a href="https://tandem.net/es" target="_blank" rel="noopener noreferrer">Tandem</a></li>
          <li><a href="https://www.hellotalk.com" target="_blank" rel="noopener noreferrer">HelloTalk</a></li>
          <li><a href="https://www.episoden.com" target="_blank" rel="noopener noreferrer">Episoden</a></li>
          <li><a href="https://www.speaky.com" target="_blank" rel="noopener noreferrer">Speaky</a> <span class="warning-tag">⚠️</span> <span class="note-tag">En exploración.</span></li>
          <li><a href="https://www.lingbe.com" target="_blank" rel="noopener noreferrer">Lingbe</a> (Apps disponibles)</li>
          <li><a href="https://www.conversationexchange.com" target="_blank" rel="noopener noreferrer">Conversation Exchange</a></li>
          <li><a href="https://language.exchange" target="_blank" rel="noopener noreferrer">Language.exchange</a></li>
          <li>Discord: Busca servidores dedicados.</li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Clases y Tutores <span class="price-tag">De Pago</span></h4>
        <ul>
          <li><img src="{{ '/assets/logo-italki.png' | relative_url }}" alt="Logo italki" class="resource-logo"><a href="https://www.italki.com/es" target="_blank" rel="noopener noreferrer">italki</a></li>
          <li><a href="https://www.cambly.com/english?lang=es" target="_blank" rel="noopener noreferrer">Cambly</a></li>
        </ul>
      </div>
    </div>
    <div class="resource-category">
        <h3>Mejora de Pronunciación</h3>
        <div class="resource-item">
            <h4>Recursos Generales de Pronunciación:</h4>
            <ul>
                <li><a href="https://youglish.com" target="_blank" rel="noopener noreferrer">Youglish</a></li>
                <li><a href="https://forvo.com" target="_blank" rel="noopener noreferrer">Forvo</a></li>
            </ul>
        </div>
        <div class="resource-item">
            <h4>Aplicaciones y Técnicas Específicas:</h4>
            <ul>
                <li><a href="https://elsaspeak.com/en/" target="_blank" rel="noopener noreferrer">Elsa Speak (Inglés)</a> <span class="price-tag">De pago (opción gratuita limitada)</span></li>
                <li>Flow-verlapping: <a href="https://www.youtube.com/watch?v=17Z0qMuMOzA" target="_blank" rel="noopener noreferrer">Tutorial por Mr. Salas</a></li>
                <li>Shadowing: <a href="https://www.youtube.com/watch?v=8qx_hnAGc-k" target="_blank" rel="noopener noreferrer">Setup y Tutorial Óptimo</a></li>
            </ul>
        </div>
    </div>
  </section>

  <!-- APOYO EXTRA -->
  <section class="resource-section">
    <h2>💡 Apoyo Extra y Guías Adicionales</h2>
    <div class="resource-item">
      <h4><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo">Guías de Idiomas de Refold</h4>
      <ul>
        <li><a href="https://refold.la/es/get-started/" target="_blank" rel="noopener noreferrer">Ver Guías en Refold.la</a></li>
      </ul>
    </div>
    <div class="resource-item">
      <h4>AJATT (All Japanese All The Time)</h4>
      <p class="description"><span class="warning-tag">⚠️</span> <em>Enfoque muy intensivo.</em></p>
      <ul>
        <li><a href="https://tatsumoto-ren.github.io/blog/whats-ajatt.html" target="_blank" rel="noopener noreferrer">¿Qué es AJATT?</a></li>
      </ul>
    </div>
     <div class="resource-item">
      <h4>Canales de YouTube sobre Inmersión:</h4>
      <ul>
        <li><a href="https://www.youtube.com/@MrSalas" target="_blank" rel="noopener noreferrer">Mr. Salas</a></li>
        <li><a href="https://www.youtube.com/@mattvsjapan" target="_blank" rel="noopener noreferrer">Matt vs Japan</a></li>
        <li><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo"><a href="https://www.youtube.com/@Refold" target="_blank" rel="noopener noreferrer">Refold</a></li>
      </ul>
    </div>
  </section>

</main>
