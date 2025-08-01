---
layout: default
title: Guía Completa para Importar y Respaldar tu Historial en El Antimétodo Tracker
description: Aprende a migrar tus datos desde otros trackers o a crear respaldos completos de tu cuenta para tener control total sobre tu progreso.
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
    position: sticky;
    top: 12px;
    right: 12px;
    float: right;
    background-color: var(--secondary-color);
    color: white;
    border: none;
    padding: 0.5rem 0.9rem; 
    border-radius: 5px;
    cursor: pointer;
    font-size: 0.85em;
    font-family: var(--font-primary);
    z-index: 10;
}
.prompt-box-import .copy-button:hover {
    background-color: var(--accent-color);
}
.step-highlight {
    font-weight: bold;
    color: var(--accent-color);
}
</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Guía Completa: Importa y Respalda tu Progreso</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">Migra desde otros trackers o crea copias de seguridad completas.</p>
  </section>

  <section class="import-guide-section">
    <p class="page-intro">En El Antimétodo Tracker, tú tienes el control total de tus datos. Aquí te mostramos cómo puedes traer tu historial desde otras aplicaciones o crear respaldos completos de tu cuenta para tu tranquilidad.</p>

    <img src="{{ '/assets/importacion.jpg' | relative_url }}" alt="Ilustración de importación de datos" style="max-width: 500px; width: 100%; margin: 0 auto 3rem; border-radius: 10px; box-shadow: var(--shadow-lg);">

    <h3>Método 1: Importación Rápida de Horas (Recomendado para empezar)</h3>
    <p>Este método es ideal si vienes de otro tracker (como Toggl, Clockify, etc.) y quieres añadir tu total de horas de forma rápida para que tus estadísticas globales sean correctas desde el día uno, sin necesidad de importar cada registro individualmente.</p>
    <ol>
      <li>Navega a <span class="step-highlight">Configuración</span> en la aplicación.</li>
      <li>Busca la tarjeta <span class="step-highlight">"Importar Actividad Agregada"</span>.</li>
      <li><strong>Completa los campos:</strong>
        <ul>
          <li><strong>Total de Horas a Importar:</strong> El número total de horas que quieres añadir.</li>
          <li><strong>Idioma:</strong> El idioma al que corresponden esas horas.</li>
          <li><strong>Fecha de Inicio y Fin:</strong> El rango de fechas en el que se distribuirán esas horas.</li>
          <li><strong>Desglose por Sub-Actividad:</strong> Asigna porcentajes a las diferentes actividades para que la distribución sea realista (la suma debe ser 100%).</li>
        </ul>
      </li>
      <li>Haz clic en <span class="step-highlight">"Importar Horas Agregadas"</span>. ¡Listo! Tus estadísticas, días de aprendizaje y puntos se actualizarán automáticamente.</li>
    </ol>
    <div class="important-note">
        <p><strong>Nota:</strong> Este método es para agregar un volumen de horas a tu historial. No crea publicaciones en el feed social.</p>
    </div>

    <h3>Método 2: Respaldo y Restauración Completa de tu Cuenta</h3>
    <p>Este método es perfecto para crear una copia de seguridad completa de tu cuenta (perfil, historial, metas, todo) y restaurarla en otro navegador o dispositivo, o simplemente para guardar tu progreso de forma segura.</p>
    
    <h4>Para Exportar (Crear tu Respaldo):</h4>
    <ol>
        <li>Navega a <span class="step-highlight">Configuración</span> en la aplicación.</li>
        <li>Busca la tarjeta <span class="step-highlight">"Gestión de Datos"</span>.</li>
        <li>Haz clic en el botón <span class="step-highlight">"Exportar mis datos"</span>.</li>
        <li>Se descargará un archivo <code>antimetodo_backup_FECHA.json</code>. Guárdalo en un lugar seguro.</li>
    </ol>

    <h4>Para Importar (Restaurar tu Respaldo):</h4>
    <ol>
        <li>En el nuevo navegador o dispositivo, ve a <span class="step-highlight">Configuración</span> -> <span class="step-highlight">"Gestión de Datos"</span>.</li>
        <li>Haz clic en <span class="step-highlight">"Importar desde archivo"</span>.</li>
        <li>Selecciona el archivo <code>.json</code> que guardaste previamente.</li>
        <li>Confirma la acción. La aplicación se recargará con todos tus datos restaurados y sincronizados con tu cuenta.</li>
    </ol>
  </section>

</main>