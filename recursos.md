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
  /* display: flex; // Quitado para que el texto fluya normalmente si el logo es muy ancho */
  /* align-items: center; */
}
.resource-item li > .resource-logo { /* Estilo para el logo si está directamente en el LI */
    vertical-align: -5px; /* Ajuste vertical fino del logo */
    margin-right: 6px;
}

.price-tag, .free-tag, .warning-tag, .note-tag { 
  display: inline-block;
  padding: 0.2em 0.6em; 
  font-size: 0.8em;
  border-radius: 4px; 
  margin-left: 5px;
  font-weight: bold;
  vertical-align: middle; 
}
.price-tag { background-color: #ffe0b2; color: #e65100; border: 1px solid #e65100; }
.free-tag { background-color: #c8e6c9; color: #2e7d32; border: 1px solid #2e7d32; }
.warning-tag strong { color: #ef5350; } 
.note-tag { background-color: #e3f2fd; color: #0d47a1; border: 1px solid #0d47a1; }

.resource-item p.description, .resource-item .details { /* .details para info adicional */
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

.resource-logo {
  width: 20px; /* Reducido tamaño de logos un poco */
  height: 20px;
  margin-right: 6px; /* Reducido margen */
  object-fit: contain; 
  vertical-align: middle; 
  border-radius: 3px;
}
.resource-category > h3 > .resource-logo { 
    width: 24px;
    height: 24px;
    margin-right: 8px;
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
      <h4><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo">Refold Tracker <span class="note-tag">Recomendada para El Antimétodo</span></h4>
      <p class="description">Aplicación esencial para registrar tu tiempo de inmersión y estudio, ayudándote a medir tu progreso y mantener la motivación.</p>
      <ul>
        <li><a href="https://www.notion.so/refold/Descargar-la-App-de-Refold-ES-16d4fa7e6fbd4a909068c310a36df275" target="_blank" rel="noopener noreferrer">Información y Descarga (Notion de Refold)</a></li>
        <li><a href="https://play.google.com/store/apps/details?id=com.refoldla.habitsmobile&hl=en" target="_blank" rel="noopener noreferrer">Descargar en Play Store (Android)</a></li>
      </ul>
      <p class="description" style="margin-top: 0.8rem; font-style: italic; background-color: #f0e6f6; padding: 0.5rem; border-radius: 4px; border-left: 3px solid var(--secondary-color);">
        💡 **¡Ve El Antimétodo en acción!** Sígueme dentro de la app Refold Tracker buscando mi usuario: <strong>LuiseM93</strong> para ver cómo aplico el método y registro mi progreso.
      </p>
    </div>
    <div class="resource-item" style="margin-top: 1.5rem;"> <!-- Añadido un poco de margen superior para separar las alternativas -->
      <h4>Alternativas para Seguimiento de Tiempo:</h4>
      <p class="description">Aunque recomendamos Refold Tracker por su enfoque específico en el aprendizaje de idiomas, estas son otras herramientas populares:</p>
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
      <div class="resource-item">
        <h4>Descargar Anki:</h4>
        <ul>
          <li><a href="https://apps.ankiweb.net" target="_blank" rel="noopener noreferrer">PC / Mac / Linux (Web Oficial)</a></li>
          <li><a href="https://play.google.com/store/apps/details?id=com.ichi2.anki" target="_blank" rel="noopener noreferrer">AnkiDroid (Android)</a> <span class="free-tag">Gratis</span></li>
          <li><a href="https://apps.apple.com/us/app/ankimobile-flashcards/id373493387" target="_blank" rel="noopener noreferrer">AnkiMobile (iOS)</a> <span class="warning-tag">⚠️</span> <span class="price-tag">$24.99 USD aprox. (razón desconocida)</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Mazos Recomendados para Anki:</h4>
        <ul>
          <li><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo"><a href="https://refold.la/es/category/decks/" target="_blank" rel="noopener noreferrer">Mazos de Refold</a> <span class="price-tag">De paga ($20 USD)</span> - <em>Vale completamente la pena.</em></li>
          <li><a href="https://refold.link/community-deck-spanish" target="_blank" rel="noopener noreferrer">Mazo 1000 Palabras Inglés (Comunidad Refold)</a> <span class="free-tag">Gratis</span> <span class="warning-tag">⚠️</span> - <em>Basado en español.</em></li>
          <li><a href="https://ankiweb.net/shared/info/539815993" target="_blank" rel="noopener noreferrer">Mazo 1000 Palabras (Inglés a Francés)</a> <span class="free-tag">Gratis</span> <span class="warning-tag">⚠️</span> - <em>Comunidad.</em></li>
          <li><a href="https://ankiweb.net/shared/info/1366502789" target="_blank" rel="noopener noreferrer">Mazo Fonética del Francés</a> <span class="free-tag">Gratis</span></li>
        </ul>
      </div>
    </div>

    <div class="resource-category">
      <h3><img src="{{ '/assets/logo-busuu.png' | relative_url }}" alt="Logo Busuu" class="resource-logo">Plataformas de Aprendizaje Inicial</h3>
      <div class="resource-item">
        <h4>Busuu <span class="note-tag">Recomendada</span></h4>
        <ul>
          <li><a href="https://www.busuu.com/es/hp" target="_blank" rel="noopener noreferrer">Sitio Web de Busuu</a></li>
        </ul>
        <p class="platforms">Igualmente se encuentra en Play Store y iOS.</p>
      </div>
    </div>
  </section>

  <!-- ETAPA 2 -->
  <section class="resource-section">
    <h2>Etapa 2: Inmersión Total en el Idioma</h2>
    <div class="resource-category">
      <h3>Asistentes de Lectura, Video y Contenido</h3>
      <div class="resource-item">
        <h4><img src="{{ '/assets/logo-language-reactor.png' | relative_url }}" alt="Logo Language Reactor" class="resource-logo">Language Reactor (Diccionario emergente)</h4>
        <ul>
          <li><a href="https://www.languagereactor.com" target="_blank" rel="noopener noreferrer">Sitio Web de Language Reactor</a></li>
          <li>Tutorial de ejemplo por Mr. Salas: <a href="https://www.youtube.com/watch?v=99JDJeCovHs" target="_blank" rel="noopener noreferrer">Ver video</a></li>
        </ul>
      </div>
       <div class="resource-item">
        <h4><img src="{{ '/assets/logo-lingq.png' | relative_url }}" alt="Logo LingQ" class="resource-logo">LingQ</h4>
        <p class="description">Herramienta muy poderosa para aprender idioma mediante la lectura, la puedes utilizar en cualquier etapa del Antimétodo y es para leer a la vez que escuchas como se lee en el idioma.</p>
        <ul>
            <li><a href="https://www.lingq.com/en/" target="_blank" rel="noopener noreferrer">Sitio Web de LingQ</a> <span class="price-tag">De paga (opción gratuita limitada)</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Readlang</h4>
        <p class="description">Alternativa a LingQ para lectura. <span class="warning-tag">⚠️</span> <span class="note-tag">Recurso en exploración (no probado por el autor pero recomendado).</span></p>
        <ul>
            <li><a href="https://readlang.com" target="_blank" rel="noopener noreferrer">Sitio Web de Readlang</a> <span class="price-tag">De paga ($6 USD/mes, con versión limitada gratuita)</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Lute (Alternativa Gratuita a LingQ)</h4>
        <ul>
            <li>Tutorial de Lute por Refold: <a href="https://www.youtube.com/watch?v=mN6kUfrKpvk" target="_blank" rel="noopener noreferrer">Ver video</a></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Voracious</h4>
        <p class="description">Reproductor para aprendizaje de idiomas. <span class="warning-tag">⚠️</span> <span class="note-tag">Aún no explorado pero recomendado.</span></p>
        <ul>
            <li><a href="https://voracious.app" target="_blank" rel="noopener noreferrer">Sitio Web de Voracious</a></li>
        </ul>
      </div>
    </div>

    <div class="resource-category">
        <h3>Plataformas de Streaming</h3>
        <p class="description">Sitios para encontrar series, películas y documentales.</p>
        <ul>
            <li><img src="{{ '/assets/logo-netflix.png' | relative_url }}" alt="Logo Netflix" class="resource-logo"><a href="https://www.netflix.com" target="_blank" rel="noopener noreferrer">Netflix</a></li>
            <li><a href="https://www.primevideo.com" target="_blank" rel="noopener noreferrer">Prime Video</a></li>
            <li><a href="https://www.disneyplus.com" target="_blank" rel="noopener noreferrer">Disney Plus</a></li>
            <li><img src="{{ '/assets/logo-youtube.png' | relative_url }}" alt="Logo YouTube" class="resource-logo"><a href="https://www.youtube.com" target="_blank" rel="noopener noreferrer">YouTube</a> <span class="free-tag">Gratis</span></li>
            <li><a href="https://www.france.tv" target="_blank" rel="noopener noreferrer">France.tv</a> <span class="free-tag">Gratis</span> - <em>Sitio de streaming para ver contenido en francés (De Francia).</em></li>
        </ul>
    </div>
     <div class="resource-category">
        <h3>VPN (Para Acceder a Contenido Geobloqueado)</h3>
        <div class="resource-item">
            <h4><img src="{{ '/assets/logo-urban-vpn.png' | relative_url }}" alt="Logo Urban VPN" class="resource-logo">Urban VPN <span class="free-tag">Gratuita</span></h4>
            <p class="description">Encuentra contenido en tu idioma cambiando tu ubicación.</p>
            <ul>
                <li><a href="https://www.urban-vpn.com" target="_blank" rel="noopener noreferrer">Sitio Web de Urban VPN</a></li>
            </ul>
            <p class="platforms">Disponible en Play Store y App Store.</p>
        </div>
    </div>
    <div class="resource-category">
        <h3>Consejos de Inmersión</h3>
        <ul>
            <li>De preferencia puedes crear una cuenta de YouTube en el idioma y país meta. Así como cambiar de idioma tu cuenta de Netflix y dispositivos.</li>
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
        <p class="description">Es importante que sean solo oraciones i+1 donde solo haya una palabra desconocida y a la hora de traducir la oración completa puedes utilizar una IA para tener la definición más exacta según el contexto.</p>
        <ul>
          <li>Tutorial de ejemplo (manual): <a href="https://www.youtube.com/watch?v=0TKEytorfdY" target="_blank" rel="noopener noreferrer">Ver video</a></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Herramientas para Minado Asistido/Automático:</h4>
        <ul>
            <li><a href="https://migaku.com" target="_blank" rel="noopener noreferrer">Migaku</a> <span class="price-tag">De paga ($10 USD/mes)</span> - <em>Minado de oraciones automática con video y audio.</em></li>
            <li><a href="https://yomitan.wiki" target="_blank" rel="noopener noreferrer">Yomitan (Extensión)</a> <span class="free-tag">Gratuito</span> <span class="warning-tag">⚠️</span> - <em>Solo mina las palabras en definiciones exactas; es recomendable minar manualmente para tener la definición correcta según la oración completa y el contexto.</em></li>
        </ul>
      </div>
    </div>
  </section>
  
  <!-- INMERSIÓN PASIVA -->
  <section class="resource-section">
    <h2>Inmersión Pasiva (Recomendada desde Etapa 2)</h2>
    <div class="resource-item">
      <h4>Podcasts:</h4>
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
        </ul>
        <p class="platforms">Aplicaciones disponibles en Play Store y App Store.</p>
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
          <li><img src="{{ '/assets/logo-chatgpt.png' | relative_url }}" alt="Logo ChatGPT" class="resource-logo"><a href="https://chatgpt.com" target="_blank" rel="noopener noreferrer">ChatGPT</a> - <em>Conversación escrita o oral.</em></li>
          <li><a href="https://character.ai" target="_blank" rel="noopener noreferrer">Character.ai</a> - <em>Conversación escrita o oral.</em></li>
          <li><a href="https://www.issen.com/es/" target="_blank" rel="noopener noreferrer">Issen (Tutor IA)</a> <span class="price-tag">De paga</span></li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Intercambio de Idiomas con Nativos <span class="free-tag">Gratis</span></h4>
        <ul>
          <li><img src="{{ '/assets/logo-tandem.png' | relative_url }}" alt="Logo Tandem" class="resource-logo"><a href="https://tandem.net/es" target="_blank" rel="noopener noreferrer">Tandem</a> - <em>Habla gratis con nativos.</em></li>
          <li><a href="https://www.hellotalk.com" target="_blank" rel="noopener noreferrer">HelloTalk</a></li>
          <li><a href="https://www.episoden.com" target="_blank" rel="noopener noreferrer">Episoden</a></li>
          <li><a href="https://www.speaky.com" target="_blank" rel="noopener noreferrer">Speaky</a> <span class="warning-tag">⚠️</span> <span class="note-tag">Aún no explorado pero recomendado.</span></li>
          <li><a href="https://www.lingbe.com" target="_blank" rel="noopener noreferrer">Lingbe</a> - <em>Llamadas con nativos.</em> (Apps en Play Store y App Store)</li>
          <li><a href="https://www.conversationexchange.com" target="_blank" rel="noopener noreferrer">Conversation Exchange</a></li>
          <li><a href="https://language.exchange" target="_blank" rel="noopener noreferrer">Language.exchange</a></li>
          <li>Discord: Puedes buscar grupos donde hablen tu idioma meta.</li>
        </ul>
      </div>
      <div class="resource-item">
        <h4>Clases y Tutores <span class="price-tag">De Pago</span></h4>
        <ul>
          <li><img src="{{ '/assets/logo-italki.png' | relative_url }}" alt="Logo italki" class="resource-logo"><a href="https://www.italki.com/es" target="_blank" rel="noopener noreferrer">italki</a> - <em>Habla con nativos en tu idioma meta.</em></li>
          <li><a href="https://www.cambly.com/english?lang=es" target="_blank" rel="noopener noreferrer">Cambly</a></li>
        </ul>
      </div>
    </div>
    <div class="resource-category">
        <h3>Mejora de Pronunciación</h3>
        <div class="resource-item">
            <h4>Recursos Generales de Pronunciación:</h4>
            <ul>
                <li><a href="https://youglish.com" target="_blank" rel="noopener noreferrer">Youglish</a> - <em>Revisa pronunciación de palabras en contenido real.</em></li>
                <li><a href="https://forvo.com" target="_blank" rel="noopener noreferrer">Forvo</a> - <em>Revisa pronunciación de palabras por nativos.</em></li>
            </ul>
        </div>
        <div class="resource-item">
            <h4>Aplicaciones y Técnicas Específicas:</h4>
            <ul>
                <li><a href="https://elsaspeak.com/en/" target="_blank" rel="noopener noreferrer">Elsa Speak (Inglés)</a> <span class="price-tag">De pago (opción gratuita limitada)</span> - <em>Aprende fonética y mejora tu pronunciación en inglés.</em></li>
                <li>Flow-verlapping: <a href="https://www.youtube.com/watch?v=17Z0qMuMOzA" target="_blank" rel="noopener noreferrer">Tutorial por Mr. Salas</a> - <em>Mejora la pronunciación de forma sencilla grabando fragmentos y repitiendo.</em></li>
                <li>Shadowing: <a href="https://www.youtube.com/watch?v=8qx_hnAGc-k" target="_blank" rel="noopener noreferrer">Setup y Tutorial Óptimo</a> - <em>No es necesario para hacer shadowing pero lo puede hacer más óptimo y beneficioso.</em></li>
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
      <p class="description"><span class="warning-tag">⚠️</span> <em>Método obsesivo para aprender japonés dedicando más de 5 horas al día.</em></p>
      <ul>
        <li><a href="https://tatsumoto-ren.github.io/blog/whats-ajatt.html" target="_blank" rel="noopener noreferrer">¿Qué es AJATT? (Explicación en Tatsumoto Ren)</a></li>
      </ul>
    </div>
     <div class="resource-item">
      <h4>Canales de YouTube (Inmersión y Aprendizaje de Idiomas):</h4>
      <ul>
        <li><a href="https://www.youtube.com/@MrSalas" target="_blank" rel="noopener noreferrer">Mr. Salas</a></li>
        <li><a href="https://www.youtube.com/@mattvsjapan" target="_blank" rel="noopener noreferrer">Matt vs Japan</a></li>
        <li><img src="{{ '/assets/logo-refold.png' | relative_url }}" alt="Logo Refold" class="resource-logo"><a href="https://www.youtube.com/@Refold" target="_blank" rel="noopener noreferrer">Refold</a></li>
      </ul>
    </div>
  </section>

</main>
