---
layout: default
title: Test de Ubicación - ¿En Qué Etapa del Antimétodo Empezar?
description: Descubre tu punto de partida ideal en El Antimétodo con esta guía interactiva asistida por Inteligencia Artificial y comienza a aprender idiomas eficientemente.
---

<style>
.test-ubicacion-section {
  margin-bottom: 2.5rem;
  padding: 1.8rem;
  background-color: var(--card-background);
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.07);
}
.test-ubicacion-section h2, .test-ubicacion-section h3 {
  text-align: center;
  color: var(--primary-color);
}
.test-ubicacion-section h3 {
  color: var(--secondary-color);
  font-size: 1.4em;
  margin-top: 2rem;
  margin-bottom: 1rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px dashed var(--light-purple-color);
}
.test-ubicacion-section .intro-text {
  font-size: 1.1em;
  text-align: center;
  color: var(--text-light-color);
  margin-bottom: 2rem;
  line-height: 1.7;
}
.test-ubicacion-section .step-container {
  margin-bottom: 2.5rem;
  padding-bottom: 2rem;
  border-bottom: 1px solid var(--light-purple-color);
}
.test-ubicacion-section .step-container:last-child {
  border-bottom: none;
  margin-bottom: 0;
}
.step-title {
  display: flex;
  align-items: center;
  font-size: 1.3em; /* Ligeramente más grande */
  font-weight: 600;
  color: var(--primary-color);
  margin-bottom: 1rem;
}
.step-icon { /* Para los iconos de los pasos */
  width: 36px;
  height: 36px;
  margin-right: 12px;
  object-fit: contain; /* Asegurar que los iconos se vean bien */
}
.question-list-ubicacion {
  list-style-type: decimal;
  padding-left: 25px; /* Espacio para los números */
  margin-top: 0.5rem;
}
.question-list-ubicacion li {
  margin-bottom: 1rem;
  line-height: 1.6;
}
.prompt-box-ubicacion { /* Estilo específico para esta página si es necesario, o usa el global */
  background-color: #2d2d2d; 
  color: #f0f0f0;
  padding: 1.5rem; /* Más padding */
  border-radius: 8px; /* Más redondeado */
  font-family: 'Courier New', Courier, monospace;
  font-size: 0.95em; /* Un poco más grande el prompt */
  line-height: 1.7;
  white-space: pre-wrap; 
  word-wrap: break-word;
  margin-top: 1rem;
  position: relative;
  border: 1px solid #444;
}
.prompt-box-ubicacion .copy-button {
    position: absolute;
    top: 12px;
    right: 12px;
    background-color: var(--secondary-color);
    color: white;
    border: none;
    padding: 0.5rem 0.9rem; /* Botón un poco más grande */
    border-radius: 5px;
    cursor: pointer;
    font-size: 0.85em;
    font-family: var(--font-primary);
}
.prompt-box-ubicacion .copy-button:hover {
    background-color: var(--accent-color);
}
.prompt-box-ubicacion strong { /* Para resaltar partes del prompt */
    color: #87CEFA; /* Azul claro para el texto a reemplazar */
    font-weight: bold;
}
.final-advice {
    background-color: #e9d8f8; /* Fondo morado muy, muy pálido */
    padding: 1rem;
    border-radius: 6px;
    border-left: 4px solid var(--secondary-color);
    margin-top: 1.5rem;
}
</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Test de Ubicación Antimétodo</h1>
    <!-- Podrías poner una imagen aquí, ej: '/assets/test-ubicacion-intro.png' -->
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">¿En Qué Etapa Deberías Empezar? ¡Descúbrelo con IA!</p>
  </section>

  <section class="test-ubicacion-section">
    <p class="intro-text">¿Ya tienes conocimientos previos en el idioma que quieres aprender (o retomar) con El Antimétodo? ¡Genial! No siempre es necesario empezar desde la Etapa 1. Esta guía interactiva te ayudará, con la asistencia de la Inteligencia Artificial, a determinar cuál es el punto de partida más adecuado para ti, para que aproveches al máximo tu tiempo y disfrutes del proceso desde el primer día.</p>

    <div class="step-container">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso1-informacion.png' | relative_url }}" alt="Paso 1" class="step-icon">
        Paso 1: Tu Experiencia y Autoevaluación Inicial
      </h3>
      <p>Antes de usar la IA, reflexiona y ten lista la siguiente información sobre tu nivel actual en el idioma que quieres aprender:</p>
      <ul class="question-list-ubicacion">
        <li><strong>Idioma Meta:</strong> ¿Qué idioma es?</li>
        <li><strong>Experiencia Previa General:</strong> Describe brevemente tu experiencia previa con este idioma (ej. <em>"Estudié 2 años en la escuela hace mucho, ahora veo algunas series con subtítulos en español"</em>, <em>"Puedo leer artículos simples con ayuda de un diccionario"</em>, <em>"Viví X meses en el país pero no interactué mucho"</em>).</li>
      </ul>
      <p>Esta descripción inicial ayudará a la IA a contextualizar tus respuestas posteriores.</p>
    </div>

    <div class="step-container">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso2-prompt-ia.png' | relative_url }}" alt="Paso 2" class="step-icon">
        Paso 2: El Prompt Interactivo para la IA
      </h3>
      <p>Ahora, copia TODO el siguiente prompt (incluyendo las descripciones de las etapas) y pégalo en ChatGPT (o una IA similar). Primero, reemplaza la información <strong>[ENTRE CORCHETES Y MAYÚSCULAS]</strong> con tu propia información del Paso 1.</p>
      <p>La IA te presentará un pequeño estímulo y te hará preguntas una por una. Responde con la mayor honestidad posible.</p>
      <div class="prompt-box-ubicacion">
        <button class="copy-button" onclick="copyUbicacionPromptToClipboard()">Copiar Prompt</button>
        <span id="ubicacionPromptToCopy">Hola ChatGPT, necesito tu ayuda para determinar en qué etapa del "El Antimétodo" debería empezar a estudiar [IDIOMA META]. El Antimétodo se basa en input comprensible masivo.

Primero, necesito que actúes como un evaluador. Te describiré brevemente mi experiencia general con [IDIOMA META]: [TU EXPERIENCIA PREVIA GENERAL AQUÍ].

Luego, por favor, haz lo siguiente:
1.  **Preséntame TRES textos cortos en [IDIOMA META], uno de nivel BÁSICO, uno INTERMEDIO y uno AVANZADO.**
    *   **Texto Básico:** 2-3 frases muy simples sobre un tema cotidiano.
    *   **Texto Intermedio:** Un párrafo de 3-4 frases con vocabulario un poco más variado y estructuras ligeramente más complejas, sobre un tema general.
    *   **Texto Avanzado:** Un párrafo de 3-4 frases que podría incluir alguna expresión idiomática o jerga común (si es apropiado para [IDIOMA META], por ejemplo, en francés podrías usar algo como 'wesh' o 'choper' si encaja naturalmente), o tratar un tema un poco más abstracto.
    *(Si no puedes generar los textos directamente en [IDIOMA META] de forma fiable, describe detalladamente el contenido y la complejidad de tres escenas de video/audio distintas: una muy básica, una intermedia y una avanzada).*

2.  **Después de presentarme los TRES textos/escenas, hazme las siguientes preguntas UNA POR UNA para CADA TEXTO/ESCENA (empezando por el básico, luego intermedio, luego avanzado), esperando mi respuesta antes de pasar al siguiente texto o pregunta:**
    *   a. Para el texto [BÁSICO/INTERMEDIO/AVANZADO]: "De lo que acabas de leer/ver descrito, ¿qué tan bien sientes que entendiste el mensaje general? (Opciones: Nada/Muy Poco, Algunas Ideas Sueltas, La Idea Principal, Bastante Bien, Perfectamente)"
    *   b. Para el texto [BÁSICO/INTERMEDIO/AVANZADO]: "Si este texto/video tuviera subtítulos en [IDIOMA META], ¿cuánto te ayudarían? (Opciones: Muchísimo/Indispensables, Bastante, Un Poco, No los necesitaría)"
    *   c. Para el texto [BÁSICO/INTERMEDIO/AVANZADO]: (Solo si hubo algo de comprensión) "¿Hubo palabras o frases específicas que NO entendiste en absoluto?"

3.  **Después de mis respuestas a todas las preguntas sobre los tres textos, y considerando mi experiencia previa que te di al inicio, por favor, recomiéndame en qué etapa del Antimétodo debería enfocarme principalmente ahora y dame una justificación detallada.**

**Aquí están las 4 etapas del Antimétodo y sus criterios de entrada/foco para tu referencia:**
*   **Etapa 1: Preparación Previa** (Foco: Vocabulario base ~1000 palabras con Anki, familiarización sonidos/estructuras. Objetivo: Rampa para la inmersión. **Entrada ideal si:** la comprensión del texto BÁSICO es muy baja incluso con la idea de subtítulos, o si el usuario es principiante absoluto).
*   **Etapa 2: Inmersión Total en el Idioma** (Foco: Consumir mucho contenido auténtico CON subtítulos en idioma meta. Objetivo: Mejorar comprensión, expandir vocabulario. **Entrada ideal si:** la comprensión del texto BÁSICO e INTERMEDIO mejora significativamente CON subtítulos, y se puede disfrutar contenido simple/intermedio de esta forma. El texto AVANZADO aún puede ser difícil).
*   **Etapa 3: Free Flow Listening** (Foco: Consumir contenido SIN subtítulos, minado de oraciones i+1. Objetivo: Independizarse de subtítulos. **Entrada ideal si:** la comprensión del texto INTERMEDIO es buena o muy buena SIN subtítulos, y se puede seguir la idea principal del texto AVANZADO aunque no se entienda todo. Si la comprensión CON subtítulos en Etapa 2 ya es consistentemente alta (ej. >80-90%) en contenido variado, es momento de pasar aquí).
*   **Etapa 4: Producción del Idioma** (Foco: Activar conocimiento pasivo hablando y escribiendo. Objetivo: Fluidez. **Entrada ideal si:** la comprensión SIN subtítulos del contenido AVANZADO es muy alta (ej. >85-95%) y hay un fuerte deseo de empezar a producir activamente).

Por favor, basa tu recomendación final de etapa en mi rendimiento general a través de los tres niveles de texto y mis respuestas. Si estoy entre dos etapas, sugiere la más temprana o una transición.</p>
      </div>
    </div>
  </section>

</main>

<script>
function copyUbicacionPromptToClipboard() { // Nombre de función único
  const promptText = document.getElementById('ubicacionPromptToCopy').innerText;
  navigator.clipboard.writeText(promptText).then(() => {
    alert('¡Prompt de Ubicación copiado al portapapeles!');
  }).catch(err => {
    const textArea = document.createElement("textarea");
    textArea.value = promptText;
    document.body.appendChild(textArea);
    textArea.focus();
    textArea.select();
    try {
      document.execCommand('copy');
      alert('¡Prompt de Ubicación copiado al portapapeles! (fallback)');
    } catch (e) {
      alert('Error al copiar el prompt. Por favor, cópialo manualmente.');
      console.error('Error al copiar con fallback: ', e);
    }
    document.body.removeChild(textArea);
  });
}
</script>
