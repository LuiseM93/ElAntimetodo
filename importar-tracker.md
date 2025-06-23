---
layout: default
title: Guía: Importa tu Historial de Trackers a "El Antimétodo Tracker" con IA
description: Aprende cómo usar un prompt de IA para convertir tus datos de seguimiento de tiempo de otras apps al formato de "El Antimétodo Tracker".
---

<style>
.import-guide-section {
  margin-bottom: 2.5rem;
  padding: 1.8rem;
  background-color: var(--card-background);
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.07);
}
.import-guide-section h2, .import-guide-section h3 {
  color: var(--primary-color);
  text-align: left; 
}
.import-guide-section h3 {
  color: var(--secondary-color);
  font-size: 1.4em;
  margin-top: 2rem;
  margin-bottom: 1rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px dashed var(--light-purple-color);
}
.import-guide-section .page-intro {
  font-size: 1.1em;
  color: var(--text-light-color);
  margin-bottom: 2rem;
  line-height: 1.7;
}
.import-guide-section ol, .import-guide-section ul {
  padding-left: 25px;
}
.import-guide-section li {
  margin-bottom: 0.8rem;
  line-height: 1.6;
}
.import-guide-section strong {
    color: var(--primary-color);
    font-weight: 600;
}
.import-guide-section .important-note {
    background-color: #f0e6f6; 
    padding: 1rem;
    border-radius: 6px;
    border-left: 4px solid var(--secondary-color);
    margin: 1.5rem 0;
}
.prompt-box-import { 
  background-color: #2d2d2d; 
  color: #f0f0f0;
  padding: 1.5rem; 
  border-radius: 8px; 
  font-family: 'Courier New', Courier, monospace;
  font-size: 0.9em; 
  line-height: 1.6;
  white-space: pre-wrap; 
  word-wrap: break-word;
  margin-top: 1rem;
  border: 1px solid #444;
  max-height: 600px; 
  overflow-y: auto; 
  position: relative;
}
.prompt-box-import .copy-button {
    position: sticky; /* Para que se mantenga visible al scrollear el prompt */
    top: 12px;
    right: 12px;
    float: right; /* Alinearlo a la derecha dentro del flujo */
    background-color: var(--secondary-color);
    color: white;
    border: none;
    padding: 0.5rem 0.9rem; 
    border-radius: 5px;
    cursor: pointer;
    font-size: 0.85em;
    font-family: var(--font-primary);
    z-index: 10; /* Asegurar que esté sobre el texto del prompt */
}
.prompt-box-import .copy-button:hover {
    background-color: var(--accent-color);
}
.prompt-box-import strong.placeholder { 
    color: #87CEFA; 
    background-color: rgba(135, 206, 250, 0.15);
    padding: 0.1em 0.3em;
    border-radius: 3px;
    font-weight: bold;
}
.step-highlight {
    font-weight: bold;
    color: var(--accent-color);
}
.code-block-in-prompt { /* Para los JSON dentro del prompt */
    display: block;
    background-color: #3a3a3a;
    padding: 0.5rem;
    border-radius: 4px;
    margin: 0.5rem 0;
    font-size: 0.95em;
}
</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Guía: Importa tu Historial a "El Antimétodo Tracker"</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">Usa el poder de la IA para convertir tus datos de otros trackers.</p>
  </section>

  <section class="import-guide-section">
    <p class="page-intro">¿Has estado registrando tu aprendizaje de idiomas en otra aplicación (como Toggl, Clockify, etc.) y quieres pasarte a "El Antimétodo Tracker" sin perder tu valioso progreso? ¡Esta guía te enseñará cómo usar una Inteligencia Artificial (como ChatGPT, Gemini, Claude, etc.) para convertir tus datos!</p>

    <h3>¿Qué Necesitarás?</h3>
    <ul>
      <li><strong>Tu archivo de datos exportado:</strong> Desde tu tracker actual, exporta tu historial de actividades. El formato más común y recomendado es <strong>CSV</strong>. Algunas apps también exportan a JSON.</li>
      <li><strong>El Idioma de las Actividades:</strong> Debes saber a qué idioma corresponden los datos de tu archivo (ej. "Francés", "Inglés").</li>
      <li><strong>Acceso a una Herramienta de IA:</strong> Como ChatGPT, Google Gemini, Claude, o similar, donde puedas pegar texto y obtener una respuesta.</li>
      <li><strong>El Prompt Mágico:</strong> Te lo proporcionaremos a continuación.</li>
    </ul>

    <h3>Pasos para la Conversión con IA:</h3>
    <ol>
      <li>
        <span class="step-highlight">Prepara tu Archivo de Datos:</span> Abre tu archivo CSV o JSON exportado en un editor de texto simple (como Bloc de Notas en Windows, TextEdit en Mac, o VS Code). Selecciona TODO su contenido y cópialo. Este será el texto que pegarás donde el prompt indica <code style="background-color: #eee; padding: 0.1em 0.3em; border-radius:3px;">{{CONTENIDO_DEL_ARCHIVO_SUBIDO_POR_EL_USUARIO_COMO_STRING}}</code>.
      </li>
      <li>
        <span class="step-highlight">Copia el Siguiente Prompt Completo:</span> Este prompt contiene todas las instrucciones para la IA.
        <div class="prompt-box-import">
          <button class="copy-button" onclick="copyImportPrompt()">Copiar Prompt</button>
          <span id="importPromptToCopy">Eres una IA asistente experta en procesar datos de seguimiento de tiempo y adaptarlos al formato específico de la aplicación "El Antimétodo Tracker". Tu tarea es convertir los datos de actividad proporcionados por el usuario, que provienen de un export genérico (probablemente CSV ο JSON), en un array de objetos JSON compatibles con "El Antimétodo Tracker".

**Objetivo Principal:**
Transformar los datos del usuario en un array de objetos ActivityLogEntry según la estructura de "El Antimétodo Tracker". Solo incluye entradas que parezcan estar relacionadas con el aprendizaje de idiomas. Omite entradas genéricas de trabajo o proyectos no relacionados.

**Estructura JSON de Salida para ActivityLogEntry ("El Antimétodo Tracker"):**
Cada objeto en el array de salida debe seguir este formato:
<pre class="code-block-in-prompt">{
  "id": "string", // Genera un ID único para cada entrada (ej: new Date().toISOString() + Math.random().toString(36).substr(2, 9)).
  "language": "{{IDIOMA_SELECCIONADO_POR_USUARIO}}", // Usa el valor proporcionado.
  "category": "ActivityCategory", // DEBE ser una de: "Inmersión Activa", "Inmersión Pasiva", "Estudio Activo", "Producción".
  "subActivity": "string", // Nombre específico. Mapear a predefinida si coincide, sino usar original limpia.
  "durationMinutes": "number", // Duración total en MINUTOS (entero).
  "date": "string", // Fecha en formato ISO: "YYYY-MM-DD".
  "startTime": "string", // Opcional: HH:MM (24h). Omitir si no disponible.
  "notes": "string" // Opcional: Descripción original completa si subActivity es predefinida o si la original es muy larga.
}</pre>

**Actividades Predefinidas de "El Antimétodo" (para guiar subActivity y category):**
Esta lista es tu referencia principal. El campo "name" de estos objetos es el candidato ideal para subActivity si la descripción del usuario coincide. El campo "category" asociado es CRUCIAL.
<pre class="code-block-in-prompt">[
  { "name": "Estudio de vocabulario Anki", "description": "Consiste en el aprendizaje de nuevas palabras y frases utilizando aplicaciones de repetición espaciada como Anki, a menudo con mazos de las palabras más comunes.", "category": "Estudio Activo", "skill": "Study" },
  { "name": "Uso de apps de idiomas para bases (ej. Busuu)", "description": "Implica el uso de herramientas digitales que ayudan a construir las bases iniciales del idioma de forma guiada.", "category": "Estudio Activo", "skill": "Study" },
  { "name": "Fonética (opcional y recomendada)", "description": "Se refiere a realizar sesiones breves para familiarizarse con los sonidos y la pronunciación del idioma.", "category": "Estudio Activo", "skill": "Study" },
  { "name": "Gramática (opcional, como apoyo básico si disfrutas estudiarla)", "description": "El estudio formal de la gramática no es el foco principal, pero puede usarse de forma opcional como apoyo básico para comprender mejor las estructuras, o para refinar detalles en etapas más avanzadas, si el estudiante lo disfruta.", "category": "Estudio Activo", "skill": "Study" },
  { "name": "Estudio del sistema de escritura (Si es necesario)", "description": "Se dedica a aprender el sistema de escritura del idioma, lo cual puede ser un proceso rápido en la mayoría de los casos.", "category": "Estudio Activo", "skill": "Study" },
  { "name": "Lectura (Libros, artículos)", "description": "Consumir contenido escrito auténtico en el idioma meta, como libros o artículos, para aprender de forma natural a través del input comprensible.", "category": "Inmersión Activa", "skill": "Reading" },
  { "name": "Lectura más audio (Libro + Audiolibro)", "description": "Consumir contenido que combina texto y audio, como leer un libro mientras se escucha su audiolibro, lo que permite asociar la forma escrita con la pronunciación.", "category": "Inmersión Activa", "skill": "Reading" },
  { "name": "Inmersión intensiva con subtítulos (revisar palabras)", "description": "Consiste en consumir contenido con subtítulos en el idioma meta, prestando mucha atención para deducir el significado por el contexto y, en ocasiones, utilizando herramientas de apoyo para revisar palabras específicas. Principalmente visual y auditivo.", "category": "Inmersión Activa", "skill": "Reading" },
  { "name": "Inmersión con subtítulos freeflow", "description": "Implica consumir contenido con subtítulos en el idioma meta, pero sin detenerse a buscar cada palabra desconocida, permitiendo que el aprendizaje ocurra de forma más fluida y natural por el contexto.", "category": "Inmersión Activa", "skill": "Reading" },
  { "name": "Free Flow Listening (sin subtítulos)", "description": "Se enfoca en escuchar y comprender el idioma sin el apoyo de subtítulos, desarrollando la habilidad de entender el habla natural. Puede ser TV, YouTube, podcasts, etc.", "category": "Inmersión Activa", "skill": "Listening" },
  { "name": "Intensive Listening (opcional)", "description": "Implica escuchar repetidamente un diálogo corto (hasta tres veces), luego leer su transcripción y finalmente volver a escucharlo para una comprensión profunda.", "category": "Inmersión Activa", "skill": "Listening" },
  { "name": "Videojuegos (con subtítulos en idioma meta)", "description": "Jugar videojuegos con diálogos y textos en el idioma meta, utilizando subtítulos en el mismo idioma para reforzar la lectura y la asociación audio-texto.", "category": "Inmersión Activa", "skill": "Reading" },
  { "name": "Videojuegos (audio en idioma meta, sin subtítulos)", "description": "Jugar videojuegos con el audio en el idioma meta, centrándose en la comprensión auditiva sin la ayuda de subtítulos.", "category": "Inmersión Activa", "skill": "Listening" },
  { "name": "Inmersión Pasiva (podcasts, música de fondo)", "description": "Consiste en exponerse al idioma de fondo, prestando atención parcial, como escuchar podcasts o música mientras se realizan otras actividades, para aumentar la exposición general.", "category": "Inmersión Pasiva", "skill": "Listening" },
  { "name": "Minado de oraciones (i+1) con Anki", "description": "Consiste en crear tarjetas de Anki con oraciones completas que contengan solo una palabra nueva, incluyendo una imagen y la traducción, para aprender vocabulario en contexto.", "category": "Estudio Activo", "skill": "Study" },
  { "name": "Actividades de escritura (ej. llevar un diario)", "description": "Implica practicar la expresión escrita en el idioma, como llevar un diario o simplemente escribir textos cortos para activar el conocimiento pasivo.", "category": "Producción", "skill": "Writing" },
  { "name": "Conversación con Inteligencia Artificial (IA)", "description": "Se refiere a interactuar verbalmente o por escrito con una IA para practicar la fluidez conversacional, donde la IA puede corregir y mantener el flujo de la conversación.", "category": "Producción", "skill": "Speaking" },
  { "name": "Hablar consigo mismo (mentalmente o en voz alta)", "description": "Consiste en practicar la producción oral del idioma de forma individual, ya sea pensando en el idioma o hablando en voz alta con uno mismo.", "category": "Producción", "skill": "Speaking" }
]
</pre>
*(Nota para el prompt: Las descripciones de las actividades predefinidas deben incluirse completas en el prompt que se envía a la IA para un mejor mapeo).*

**Reglas para Analizar los Datos de Entrada del Usuario:**
1.  **Formato del Archivo:** Datos de entrada serán cadena de texto (CSV o array JSON).
    *   CSV: Primera fila puede ser encabezado ("Date", "Start Time", "Duration", "Description", "Task", "Project", "Usuario", "Email"). Identificar columnas relevantes.
    *   JSON: Array de objetos, cada uno un registro de tiempo.
2.  **Fecha (date):** Identificar y convertir a "YYYY-MM-DD". Si inválida/no parseable, omitir entrada o usar "1970-01-01" + nota explicativa.
3.  **Duración (durationMinutes):** Convertir formatos ("HH:MM:SS", "HH:MM", minutos, horas decimales como 1.5) a MINUTOS totales enteros. Si falta/inválida, omitir o usar 1 minuto + nota.
4.  **Descripción / Nombre de Tarea (para subActivity y notes): CAMPO CLAVE.**
    *   **Mapeo de subActivity:** Comparar descripción del usuario con "name" de actividades predefinidas (ignorar mayúsculas/minúsculas). Si hay coincidencia razonable, usar ese "name". Si no, usar descripción original limpia (sin espacios extra).
    *   **Determinación de category:**
        *   Si subActivity mapeó a predefinida, USAR SU "category" asociada.
        *   Si subActivity es personalizada, INFERIR "category" basándose en descripción y filosofía del Antimétodo (Palabras clave: "Inmersión Activa": viendo, leyendo, jugando, podcast atento, YouTube profundo, anime, serie, película, libro, documental. "Inmersión Pasiva": escucha de fondo, música mientras trabajo, podcast mientras cocino. "Estudio Activo": Anki, Duolingo, Busuu, gramática, vocabulario, repaso, lección app, minando, tarjetas. "Producción": conversación, hablando, escribiendo, intercambio, clase con tutor, diario, chat nativo, clase conversación).
    *   **IMPORTANTE:** Si la descripción NO ESTÁ RELACIONADA con aprendizaje de idiomas (ej: "Reunión de cliente", "Desarrollo de software", "Compras"), OMITE esa entrada.
    *   **Campo notes:** Si subActivity es predefinida, usar descripción original completa como notes. Si descripción original es muy larga, subActivity puede ser resumen y el resto va a notes.
5.  **Hora de Inicio (startTime):** Si disponible (ej: "14:30", "2:30 PM"), convertir a "HH:MM" (24h). Si no, omitir.
6.  **ID (id):** Generar ID único: `new Date().toISOString() + Math.random().toString(36).substr(2, 9)`.

**Lógica de Procesamiento para la IA:**
1. Parsea datos de entrada. 2. Itera sobre cada registro. 3. Extrae/transforma campos según reglas. 4. Si actividad es relevante para idiomas, construye objeto ActivityLogEntry. 5. Reúne objetos válidos en array JSON.

**Formato de Salida REQUERIDO:**
Devuelve ÚNICAMENTE la cadena de texto del array JSON final. No incluyas explicaciones, texto adicional, ni markdown. La respuesta debe ser directamente parseable como JSON.

**A continuación, te proporcionaré los DATOS DEL USUARIO y el IDIOMA META.**

--- Comienza la conversión después de recibir los siguientes dos bloques de información ---

**Datos del Usuario (el contenido de su archivo exportado):**
<strong class="placeholder">{{CONTENIDO_DEL_ARCHIVO_SUBIDO_POR_EL_USUARIO_COMO_STRING}}</strong>

**Idioma Meta para estas Actividades:**
<strong class="placeholder">{{IDIOMA_SELECCIONADO_POR_USUARIO}}</strong>
</span>
        </div>
      </li>
      <li>
        <span class="step-highlight">Prepara tu Información Adicional:</span> En una nueva línea en tu herramienta de IA (después de pegar el prompt anterior), escribe y reemplaza:
        <ul style="list-style-type: square; margin-top:0.5rem;">
            <li>El texto <code style="background-color: #eee; padding: 0.1em 0.3em; border-radius:3px;">{{CONTENIDO_DEL_ARCHIVO_SUBIDO_POR_EL_USUARIO_COMO_STRING}}</code> con el contenido completo de tu archivo CSV o JSON (el que copiaste en el Paso 1).</li>
            <li>Luego, el texto <code style="background-color: #eee; padding: 0.1em 0.3em; border-radius:3px;">{{IDIOMA_SELECCIONADO_POR_USUARIO}}</code> con el idioma al que corresponden esas actividades (ej. `Francés`).</li>
        </ul>
        <p><em>Ejemplo de cómo se vería al final de lo que pegas en la IA (después del prompt largo):</em></p>
        <pre style="background-color: #eee; padding: 0.5rem; border-radius: 4px; font-size:0.85em; color: #333;">... (final del prompt copiado arriba, terminando en "...IDIOMA_SELECCIONADO_POR_USUARIO}}")

Fecha,Descripción,Duración
2024-01-01,Ver serie Netflix,0:45:00
2024-01-01,Anki Repaso,0:15:00
2024-01-02,Podcast mientras cocino,0:30:00

Francés</pre>
        <p><em>Nota: La parte de "Datos del Usuario" y "Idioma Meta para estas Actividades" NO forma parte del prompt que copias con el botón, sino que son las instrucciones para que el usuario añada su información DESPUÉS de pegar el prompt en la IA. He modificado el prompt para que la IA espere estos dos bloques de información.</em></p>
      </li>
      <li>
        <span class="step-highlight">Envía Todo a la IA:</span> Una vez que hayas pegado el prompt principal y luego tus datos y el idioma, envía la solicitud completa a la IA.
      </li>
      <li>
        <span class="step-highlight">Obtén tu JSON:</span> La IA debería devolverte un bloque de texto que es un array JSON. Cópialo.
      </li>
      <li>
        <span class="step-highlight">Importa a "El Antimétodo Tracker":</span> Guarda ese texto JSON en un nuevo archivo con extensión `.json` (ej. `antimetodo_importado.json`) en tu computadora. Luego, ve a la Configuración de la app "El Antimétodo Tracker" e importa este nuevo archivo. ¡Listo! Tu historial estará en tu nuevo tracker.
      </li>
    </ol>

    <div class="important-note">
      <h4><span class="warning-tag">⚠️</span> Consideraciones Importantes:</h4>
      <ul>
        <li><strong>Límites de la IA:</strong> Si tu archivo de datos es MUY grande, podrías alcanzar el límite de caracteres de la ventana de prompt de la IA. En ese caso, intenta procesar tus datos en tandas más pequeñas.</li>
        <li><strong>Calidad de la Conversión:</strong> La IA es inteligente, pero no infalible. Revisa siempre los datos importados en "El Antimétodo Tracker" y haz ajustes manuales si es necesario. Cuanto más claras sean las descripciones en tu archivo original, mejor será el resultado.</li>
        <li><strong>Privacidad:</strong> Recuerda que estás pegando tus datos en una herramienta de IA de terceros. Revisa sus políticas de privacidad si te preocupa la sensibilidad de tu información.</li>
      </ul>
    </div>
  </section>

</main>

<script>
function copyImportPrompt() {
  const promptText = document.getElementById('importPromptToCopy').innerText;
  navigator.clipboard.writeText(promptText).then(() => {
    alert('¡Prompt para la IA copiado al portapapeles!\n\nRecuerda pegar tus datos y el idioma después de este prompt en la IA.');
  }).catch(err => {
    const textArea = document.createElement("textarea");
    textArea.value = promptText;
    document.body.appendChild(textArea);
    textArea.focus();
    textArea.select();
    try {
      document.execCommand('copy');
      alert('¡Prompt para la IA copiado al portapapeles! (fallback)\n\nRecuerda pegar tus datos y el idioma después de este prompt en la IA.');
    } catch (e) {
      alert('Error al copiar el prompt. Por favor, cópialo manualmente.');
      console.error('Error al copiar con fallback: ', e);
    }
    document.body.removeChild(textArea);
  });
}
</script>
