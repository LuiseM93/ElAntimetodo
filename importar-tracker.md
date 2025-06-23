---
layout: default
title: Importar Historial de Otros Trackers - El Antimétodo Tracker
description: Transfiere fácilmente tu progreso de aprendizaje de idiomas desde otras aplicaciones de seguimiento de tiempo a "El Antimétodo Tracker" con nuestra herramienta de importación asistida por IA.
---

<style>
.import-tool-section {
  margin-bottom: 2.5rem;
  padding: 1.8rem;
  background-color: var(--card-background);
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.07);
}
.import-tool-section h2, .import-tool-section h3 {
  color: var(--primary-color);
  text-align: left; /* Alinear a la izquierda para contenido más técnico */
}
.import-tool-section h3 {
  color: var(--secondary-color);
  font-size: 1.4em;
  margin-top: 2rem;
  margin-bottom: 1rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px dashed var(--light-purple-color);
}
.import-tool-section .page-intro {
  font-size: 1.1em;
  color: var(--text-light-color);
  margin-bottom: 2rem;
  line-height: 1.7;
}
.import-tool-section ol, .import-tool-section ul {
  padding-left: 25px;
}
.import-tool-section li {
  margin-bottom: 0.8rem;
  line-height: 1.6;
}
.import-tool-section strong { /* Para resaltar en listas */
    color: var(--primary-color);
    font-weight: 600;
}
.import-tool-section .privacy-note, .import-tool-section .conversion-tips {
    background-color: #f0e6f6; /* Morado muy pálido */
    padding: 1rem;
    border-radius: 6px;
    border-left: 4px solid var(--secondary-color);
    margin-top: 1.5rem;
    margin-bottom: 1.5rem;
}
.import-tool-section .ui-controls-list li {
    list-style-type: '▶️'; /* Viñeta diferente para controles UI */
    padding-left: 0.5em;
}
.prompt-display-box {
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
  max-height: 500px; /* Para que no sea excesivamente largo */
  overflow-y: auto; /* Scroll si el prompt es muy largo */
}
.prompt-display-box strong { /* Para placeholders en el prompt */
    color: #87CEFA; 
    font-weight: bold;
}
.json-structure-box {
  background-color: #f9f9f9;
  border: 1px solid #e0e0e0;
  padding: 1rem;
  border-radius: 6px;
  font-family: 'Courier New', Courier, monospace;
  font-size: 0.85em;
  white-space: pre-wrap;
  margin-top: 0.5rem;
}
</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Importa tu Historial de Otros Trackers</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">Transfiere tu progreso a "El Antimétodo Tracker" fácilmente.</p>
  </section>

  <section class="import-tool-section">
    <p class="page-intro">¿Has estado registrando tu aprendizaje de idiomas en otra aplicación (como Toggl, Clockify, u otras) y quieres pasarte a "El Antimétodo Tracker" sin perder tu progreso? ¡Esta herramienta (próximamente interactiva en esta página) te ayudará a hacerlo!</p>

    <h3>¿Cómo Funcionará?</h3>
    <ol>
      <li><strong>Exporta tus Datos:</strong> Desde tu tracker actual, exporta tu historial de actividades. El formato más común y recomendado es <strong>CSV</strong>. Algunas apps también exportan a JSON.</li>
      <li><strong>Sube tu Archivo:</strong> (Próximamente) Podrás cargar el archivo CSV (o JSON) que exportaste directamente aquí.</li>
      <li><strong>Selecciona el Idioma:</strong> Indica a qué idioma corresponden las actividades de este archivo. Esto es crucial para "El Antimétodo Tracker".</li>
      <li><strong>Magia de IA:</strong> Nuestra IA (Gemini o similar) analizará tu archivo e intentará asignar cada actividad a las categorías y sub-actividades de "El Antimétodo".</li>
      <li><strong>Descarga y Listo:</strong> Te daremos un nuevo archivo JSON formateado específicamente para "El Antimétodo Tracker". Simplemente ve a la Configuración de la app "El Antimétodo Tracker" e importa este nuevo archivo.</li>
    </ol>

    <div class="conversion-tips">
      <h4>Consejos para una Mejor Conversión:</h4>
      <ul>
        <li><strong>Descripciones Claras:</strong> Cuanto más descriptivos fueran los nombres de tus actividades en el tracker original (ej. "Ver serie en Netflix - Francés" en lugar de solo "Netflix"), mejor podrá la IA categorizarlas.</li>
        <li><strong>Formatos Soportados:</strong> Preferimos archivos CSV. Si usas JSON, asegúrate de que sea un array de registros de tiempo.</li>
        <li><strong>Revisión Post-Importación:</strong> La IA es inteligente, pero no infalible. Es posible que algunas actividades necesiten un ajuste manual después de importarlas en "El Antimétodo Tracker".</li>
      </ul>
    </div>

    <div class="privacy-note">
      <h4>Privacidad de tus Datos:</h4>
      <p>El archivo que subas solo se usará para procesar la conversión con la IA y no se almacenará de forma permanente en nuestros servidores (cuando la herramienta esté plenamente funcional).</p>
    </div>

    <h3>Controles de la Herramienta (Interfaz Propuesta):</h3>
    <p>Cuando esta herramienta esté activa en la página, encontrarás controles como:</p>
    <ul class="ui-controls-list">
        <li><strong>Botón "Seleccionar Archivo"</strong> (para CSV o JSON).</li>
        <li><strong>Lista Desplegable "Idioma de las Actividades"</strong>: (Poblada con los idiomas soportados, ej: "Español", "English", "Français", etc.).</li>
        <li><em>(Opcional, para CSV más complejos):</em> Campos para indicar qué columna es la "Fecha", "Duración", y "Descripción" si la IA no las detecta automáticamente.</li>
        <li><strong>Botón "Convertir mis Datos"</strong>.</li>
    </ul>
    <p><em>(Actualmente, esta página es informativa. La funcionalidad de carga y conversión directa se implementará en el futuro en la aplicación "El Antimétodo Tracker" o aquí mismo.)</em></p>

    <hr style="margin: 2.5rem 0;">

    <h3>Detalles Técnicos para la Conversión con IA (Referencia para el Desarrollador)</h3>
    <p>La siguiente información detalla el prompt que se enviaría a un modelo de IA (como Gemini) en el backend para procesar los datos del usuario.</p>
    
    <h4>1. El "Prompt" para la IA (Gemini)</h4>
    <p>Cuando un usuario suba su archivo y seleccione el idioma, el backend enviaría el contenido del archivo, el idioma seleccionado y el siguiente prompt a la API de la IA:</p>
    <div class="prompt-display-box">
Eres una IA asistente experta en procesar datos de seguimiento de tiempo y adaptarlos al formato específico de la aplicación "El Antimétodo Tracker". Tu tarea es convertir los datos de actividad proporcionados por el usuario, que provienen de un export genérico (probablemente CSV ο JSON), en un array de objetos JSON compatibles con "El Antimétodo Tracker".

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
