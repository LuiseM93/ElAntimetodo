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
.test-ubicacion-section h3 { /* Título de cada paso */
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
  border-bottom: 1px solid var(--light-purple-color); /* Borde sólido para separar pasos */
}
.test-ubicacion-section .step-container:last-child {
  border-bottom: none;
  margin-bottom: 0;
}
.step-title { /* Estilo para el H3 de cada paso si se usa fuera del .test-ubicacion-section h3 */
  display: flex;
  align-items: center;
  font-size: 1.3em; 
  font-weight: 600;
  color: var(--primary-color);
  margin-bottom: 1rem;
}
.step-icon { 
  width: 36px;
  height: 36px;
  margin-right: 12px;
  object-fit: contain; 
}
.question-list-ubicacion {
  list-style-type: decimal;
  padding-left: 25px; 
  margin-top: 0.5rem;
}
.question-list-ubicacion li {
  margin-bottom: 1rem;
  line-height: 1.6;
}
.prompt-box-ubicacion { 
  background-color: #2d2d2d; 
  color: #f0f0f0;
  padding: 1.5rem; 
  border-radius: 8px; 
  font-family: 'Courier New', Courier, monospace;
  font-size: 0.95em; 
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
    padding: 0.5rem 0.9rem; 
    border-radius: 5px;
    cursor: pointer;
    font-size: 0.85em;
    font-family: var(--font-primary);
}
.prompt-box-ubicacion .copy-button:hover {
    background-color: var(--accent-color);
}
.prompt-box-ubicacion strong { 
    color: #87CEFA; 
    font-weight: bold;
}
.final-advice {
    background-color: #e9d8f8; 
    padding: 1.2rem; /* Más padding */
    border-radius: 6px;
    border-left: 4px solid var(--secondary-color);
    margin-top: 1.5rem;
    font-size: 1.05em; /* Un poco más grande el texto del consejo */
}
.final-advice p {
    margin-bottom: 0.8rem;
}
.final-advice p:last-child {
    margin-bottom: 0;
}
</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Test de Ubicación Antimétodo</h1>
    <!-- <img src="{{ '/assets/test-ubicacion-intro.png' | relative_url }}" alt="Descubre tu etapa en El Antimétodo" class="test-ubicacion-intro-image"> -->
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">¿En Qué Etapa Deberías Empezar? ¡Descúbrelo con IA!</p>
  </section>

  <section class="test-ubicacion-section">
    <p class="intro-text">¿Ya tienes conocimientos previos en el idioma que quieres aprender (o retomar) con El Antimétodo? ¡Genial! No siempre es necesario empezar desde la Etapa 1. Esta guía interactiva te ayudará, con la asistencia de la Inteligencia Artificial, a determinar cuál es el punto de partida más adecuado para ti, para que aproveches al máximo tu tiempo y disfrutes del proceso desde el primer día.</p>

    <div class="step-container">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso1-informacion.png' | relative_url }}" alt="Paso 1" class="step-icon">
        Paso 1: Tu Experiencia Previa
      </h3>
      <p>Antes de usar la IA, ten lista una breve descripción de tu experiencia general con el idioma que quieres aprender/retomar. Por ejemplo:</p>
      <ul style="list-style-type: '💡'; padding-left: 20px;">
        <li><em>"Estudié francés 2 años en la escuela hace una década, recuerdo algunas palabras básicas."</em></li>
        <li><em>"Veo anime en japonés con subtítulos en español regularmente y entiendo algunas frases comunes."</em></li>
        <li><em>"Puedo leer artículos de noticias simples en inglés con algo de esfuerzo."</em></li>
      </ul>
      <p>Esta descripción inicial es la primera pieza de información que le darás a la IA.</p>
    </div>

    <div class="step-container">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso2-prompt-ia.png' | relative_url }}" alt="Paso 2" class="step-icon">
        Paso 2: Interactúa con la IA Diagnóstica
      </h3>
      <p>Ahora, copia TODO el siguiente prompt (incluyendo las descripciones de las etapas) y pégalo en ChatGPT (o una IA similar). Primero, reemplaza la información <strong>[ENTRE CORCHETES Y MAYÚSCULAS]</strong> con tu propia información del Paso 1.</p>
      <p>La IA te presentará tres pequeños estímulos (textos o descripciones de escenas) de dificultad creciente y te hará preguntas sobre ellos. Responde cada pregunta con la mayor honestidad posible.</p>
      <div class="prompt-box-ubicacion">
        <button class="copy-button" onclick="copyUbicacionPromptToClipboard()">Copiar Prompt</button>
        <span id="ubicacionPromptToCopy">Hola ChatGPT, necesito tu ayuda para determinar en qué etapa del "El Antimétodo" debería empezar a estudiar <strong>[IDIOMA META]</strong>. El Antimétodo es un método de aprendizaje de idiomas basado en input comprensible masivo.

Primero, necesito que actúes como un evaluador. Te describiré brevemente mi experiencia general con <strong>[IDIOMA META]</strong>: <strong>[TU EXPERIENCIA PREVIA GENERAL AQUÍ]</strong>.

Luego, por favor, haz lo siguiente:
1.  Preséntame TRES textos cortos en <strong>[IDIOMA META]</strong>, uno de nivel BÁSICO, uno INTERMEDIO y uno AVANZADO.
    *   Texto Básico: 2-3 frases muy simples sobre un tema cotidiano.
    *   Texto Intermedio: Un párrafo de 3-4 frases con vocabulario un poco más variado y estructuras ligeramente más complejas, sobre un tema general.
    *   Texto Avanzado: Un párrafo de 3-4 frases que podría incluir alguna expresión idiomática o jerga común (si es apropiado para <strong>[IDIOMA META]</strong>), o tratar un tema un poco más abstracto.
    (Si no puedes generar los textos directamente en <strong>[IDIOMA META]</strong> de forma fiable, describe detalladamente el contenido y la complejidad de tres escenas de video/audio distintas: una muy básica, una intermedia y una avanzada).

2.  Después de presentarme los TRES textos/escenas, hazme las siguientes preguntas UNA POR UNA para CADA TEXTO/ESCENA (empezando por el básico, luego intermedio, luego avanzado), esperando mi respuesta antes de pasar al siguiente texto o pregunta:
    *   a. Para el texto [BÁSICO/INTERMEDIO/AVANZADO]: "De lo que acabas de leer/ver descrito, ¿qué tan bien sientes que entendiste el mensaje general? (Opciones: Nada/Muy Poco, Algunas Ideas Sueltas, La Idea Principal, Bastante Bien, Perfectamente)"
    *   b. Para el texto [BÁSICO/INTERMEDIO/AVANZADO]: "Si este texto/video tuviera subtítulos en <strong>[IDIOMA META]</strong>, ¿cuánto te ayudarían? (Opciones: Muchísimo/Indispensables, Bastante, Un Poco, No los necesitaría)"
    *   c. Para el texto [BÁSICO/INTERMEDIO/AVANZADO]: (Solo si hubo algo de comprensión) "¿Hubo palabras o frases específicas que NO entendiste en absoluto?"

3.  Después de mis respuestas a todas las preguntas sobre los tres textos, y considerando mi experiencia previa que te di al inicio, por favor, recomiéndame en qué etapa del Antimétodo debería enfocarme principalmente ahora y dame una justificación detallada.

Aquí están las 4 etapas del Antimétodo y sus criterios de entrada/foco para tu referencia:
*   **Etapa 1: Preparación Previa** (Foco: Vocabulario base ~1000 palabras con Anki, familiarización sonidos/estructuras. Objetivo: Rampa para la inmersión. Entrada ideal si: la comprensión del texto BÁSICO es muy baja incluso con la idea de subtítulos, o si el usuario es principiante absoluto).
*   **Etapa 2: Inmersión Total en el Idioma** (Foco: Consumir mucho contenido auténtico CON subtítulos en idioma meta. Objetivo: Mejorar comprensión, expandir vocabulario. Entrada ideal si: la comprensión del texto BÁSICO e INTERMEDIO mejora significativamente CON subtítulos, y se puede disfrutar contenido simple/intermedio de esta forma. El texto AVANZADO aún puede ser difícil).
*   **Etapa 3: Free Flow Listening** (Foco: Consumir contenido SIN subtítulos, minado de oraciones i+1. Objetivo: Independizarse de subtítulos. Entrada ideal si: la comprensión del texto INTERMEDIO es buena o muy buena SIN subtítulos, y se puede seguir la idea principal del texto AVANZADO aunque no se entienda todo. Si la comprensión CON subtítulos en Etapa 2 ya es consistentemente alta (ej. >80-90%) en contenido variado, es momento de pasar aquí).
*   **Etapa 4: Producción del Idioma** (Foco: Activar conocimiento pasivo hablando y escribiendo. Objetivo: Fluidez. Entrada ideal si: la comprensión SIN subtítulos del contenido AVANZADO es muy alta (ej. >85-95%) y hay un fuerte deseo de empezar a producir activamente).

Por favor, basa tu recomendación final de etapa en mi rendimiento general a través de los tres niveles de texto y mis respuestas. Si estoy entre dos etapas, sugiere la más temprana o una transición.
Espera a que te dé mi experiencia previa antes de empezar con el texto/escena y las preguntas.</span>
      </div>
    </div>

    <div class="step-container" style="border-bottom:none; margin-bottom:0;">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso3-revisar-adaptar.png' | relative_url }}" alt="Paso 3" class="step-icon">
        Paso 3: Interpreta la Recomendación y ¡Empieza!
      </h3>
      <p>La Inteligencia Artificial te dará una sugerencia de etapa basada en tus respuestas. ¡Úsala como una guía valiosa!</p>
      <div class="final-advice">
        <p><strong>Recuerda:</strong> Si la IA te recomienda, por ejemplo, la Etapa 2, pero sientes que tu vocabulario base es aún muy débil, no dudes en dedicar unas semanas a las actividades clave de la Etapa 1 (como Anki con palabras frecuentes) antes de sumergirte de lleno en la inmersión. ¡Tú conoces mejor tu situación y tu ritmo!</p>
        <p>Lo más importante es que te sientas cómodo y motivado. Una vez que tengas una idea clara de tu etapa de inicio, visita nuestra descripción detallada de <a href="{{ '/etapas' | relative_url }}">Las Etapas del Antimétodo</a> y nuestra sección de <a href="{{ '/rutinas' | relative_url }}">Rutinas Flexibles</a> para comenzar a planificar tu emocionante viaje de aprendizaje.</p>
      </div>
    </div>
  </section>

</main>

<script>
function copyUbicacionPromptToClipboard() { 
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
