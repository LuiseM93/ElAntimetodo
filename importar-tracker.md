---
layout: default
title: Guía para Importar tu Historial de Trackers a "El Antimétodo Tracker" con IA
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
.prompt-box-import { /* Renombrado para evitar conflictos si usas prompt-box en otra parte */
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
  max-height: 600px; /* Aumentada altura máxima */
  overflow-y: auto; 
  position: relative;
}
.prompt-box-import .copy-button {
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
.prompt-box-import .copy-button:hover {
    background-color: var(--accent-color);
}
.prompt-box-import strong.placeholder { /* Para placeholders en el prompt */
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
        <span class="step-highlight">Prepara tu Archivo de Datos:</span> Abre tu archivo CSV o JSON exportado en un editor de texto simple (como Bloc de Notas en Windows, TextEdit en Mac, o VS Code). Selecciona TODO su contenido y cópialo. Este será el <code style="background-color: #eee; padding: 0.1em 0.3em; border-radius:3px;">{{CONTENIDO_DEL_ARCHIVO_SUBIDO_POR_EL_USUARIO_COMO_STRING}}</code>.
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
```json
[
  {
    "id": "string", // Genera un ID único para cada entrada (ej: new Date().toISOString() + Math.random().toString(36).substr(2, 9)).
    "language": "{{IDIOMA_SELECCIONADO_POR_USUARIO}}", // Usa el valor proporcionado.
    "category": "ActivityCategory", // DEBE ser una de: "Inmersión Activa", "Inmersión Pasiva", "Estudio Activo", "Producción".
    "subActivity": "string", // Nombre específico. Mapear a predefinida si coincide, sino usar original limpia.
    "durationMinutes": "number", // Duración total en MINUTOS (entero).
    "date": "string", // Fecha en formato ISO: "YYYY-MM-DD".
    "startTime": "string", // Opcional: HH:MM (24h). Omitir si no disponible.
    "notes": "string" // Opcional: Descripción original completa si subActivity es predefinida o si la original es muy larga.
  }
]
