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

/* Estilos para los inputs del usuario */
.user-input-field {
  display: block;
  width: 100%;
  padding: 0.7rem;
  margin-bottom: 1rem;
  font-family: var(--font-secondary);
  font-size: 1em;
  border: 1px solid var(--light-purple-color);
  border-radius: 5px;
  box-sizing: border-box;
}
.user-input-field:focus {
  border-color: var(--secondary-color);
  outline: none;
  box-shadow: 0 0 0 2px var(--light-purple-color);
}
label {
    display: block;
    margin-bottom: 0.3rem;
    font-weight: 500;
    color: var(--text-color);
}

.final-advice {
    background-color: #e9d8f8; 
    padding: 1.2rem; 
    border-radius: 6px;
    border-left: 4px solid var(--secondary-color);
    margin-top: 1.5rem;
    font-size: 1.05em; 
}
.final-advice p { margin-bottom: 0.8rem; }
.final-advice p:last-child { margin-bottom: 0; }
  
.interactive-button {
  background: linear-gradient(135deg, var(--secondary-color), var(--accent-color));
  color: #fff;
  font-size: 1em;
  font-weight: 600;
  font-family: var(--font-primary);
  border: none;
  padding: 0.8rem 1.4rem;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.interactive-button:hover {
  background: linear-gradient(135deg, var(--accent-color), var(--secondary-color));
  transform: translateY(-2px);
  box-shadow: 0 6px 14px rgba(0, 0, 0, 0.15);
}

.interactive-button:active {
  transform: scale(0.97);
  box-shadow: 0 3px 7px rgba(0, 0, 0, 0.1);
}
</style>

<main class="content-wrapper">

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Test de Ubicación Antimétodo</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">¿En Qué Etapa Deberías Empezar? ¡Descúbrelo con IA!</p>
  </section>

  <section class="test-ubicacion-section">
    <p class="intro-text">¿Ya tienes conocimientos previos en el idioma que quieres aprender (o retomar) con El Antimétodo? ¡Genial! No siempre es necesario empezar desde la Etapa 1. Esta guía interactiva te ayudará, con la asistencia de la Inteligencia Artificial, a determinar cuál es el punto de partida más adecuado para ti.</p>

    <div class="step-container">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso1-informacion.png' | relative_url }}" alt="Paso 1" class="step-icon">
        Paso 1: Proporciona tu Información
      </h3>
      <p>Ingresa los siguientes datos. Serán usados para generar un prompt personalizado para la IA:</p>
      
      <label for="idiomaMeta">Idioma que quieres aprender/retomar:</label>
      <input type="text" id="idiomaMeta" class="user-input-field" placeholder="Ej: Francés, Japonés, Inglés">
      
      <label for="experienciaPrevia">Describe brevemente tu experiencia previa con este idioma:</label>
      <textarea id="experienciaPrevia" class="user-input-field" rows="3" placeholder="Ej: Estudié 2 años en la escuela hace mucho, veo algunas series con subtítulos en español y entiendo frases comunes."></textarea>
      
      <button class="interactive-button" onclick="generarYMostrarPrompt()">✨ Generar Prompt para la IA</button>
    </div>

    <div class="step-container" id="paso2IA" style="display:none;">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso2-prompt-ia.png' | relative_url }}" alt="Paso 2" class="step-icon">
        Paso 2: Interactúa con la IA Diagnóstica
      </h3>
      <p>¡Excelente! Hemos generado un prompt personalizado para ti. La IA te presentará tres pequeños estímulos de dificultad creciente y te hará preguntas sobre ellos. Responde con honestidad.</p>
      <p><strong>Instrucciones:</strong> Copia el texto de abajo, pégalo en ChatGPT y vuelve aquí para completar el Paso 3.</p>
      
      <div style="position: relative; margin-top: 1rem;">
        <textarea id="ubicacionPromptToCopy" readonly class="user-input-field" style="height: 150px; font-family: monospace; font-size: 0.85em; background-color: #f8f9fa; border: 2px solid var(--secondary-color); color: #333; resize: none;"></textarea>
        <button id="btnCopiarPrompt" class="interactive-button" onclick="copyUbicacionPromptToClipboard()" style="margin-top: 0.5rem; width: 100%;">
          <span>📋 Copiar Prompt</span>
        </button>
      </div>
    </div>

    <div class="step-container" id="paso3Interpreta" style="display:none; border-bottom:none; margin-bottom:0;">
      <h3 class="step-title">
        <img src="{{ '/assets/rutinas-paso3-revisar-adaptar.png' | relative_url }}" alt="Paso 3" class="step-icon">
        Paso 3: Interpreta la Recomendación y ¡Empieza!
      </h3>
      <p>La Inteligencia Artificial te dará una sugerencia de etapa basada en tus respuestas. ¡Úsala como una guía valiosa!</p>
      <div class="final-advice">
        <p><strong>Recuerda:</strong> Si la IA te recomienda la Etapa 2, pero sientes que tu vocabulario base es aún muy débil, no dudes en dedicar unas semanas a las actividades clave de la Etapa 1 antes de sumergirte de lleno en la inmersión. ¡Tú conoces mejor tu situación!</p>
        <p>Una vez que tengas tu etapa, revisa los detalles en <a href="{{ '/etapas' | relative_url }}">Las Etapas del Antimétodo</a> para comenzar tu viaje.</p>
      </div>

      <!-- SECCIÓN DE CAPTURA DE EMAIL DESPUÉS DEL RESULTADO -->
      <div style="margin-top: 3rem; padding: 2rem; background-color: #f0e6f6; border-radius: 12px; border: 2px dashed var(--secondary-color); text-align: center;">
        <h3 style="margin-top: 0; color: var(--primary-color);">🎁 ¡Recibe tu Guía de Inicio Personalizada!</h3>
        <p style="font-size: 1.1em; color: var(--text-light-color);">Para ayudarte a arrancar con éxito en la etapa que te recomendó la IA, te enviaré por correo:</p>
        <ul style="text-align: left; display: inline-block; margin-bottom: 1.5rem;">
          <li>✅ El PDF de la <strong>Guía Esencial de El Antimétodo</strong></li>
          <li>✅ Mi <strong>Rutina Diaria de 7 meses</strong> (con la que aprendí francés)</li>
          <li>✅ Los <strong>Mazos de Anki recomendados</strong> para empezar</li>
        </ul>
        
        <div class="ml-embedded" data-form="RksRhl"></div>
      </div>
    </div>
  </section>

</main>

<script>
const promptPlantilla = `Hola ChatGPT, necesito tu ayuda para determinar en qué etapa del "El Antimétodo" debería empezar a estudiar [IDIOMA META]. El Antimétodo es un método de aprendizaje de idiomas basado en input comprensible masivo.

Primero, necesito que actúes como un evaluador. Te describiré brevemente mi experiencia general con [IDIOMA META]: [EXPERIENCIA PREVIA GENERAL].

Luego, por favor, haz lo siguiente:
1.  Preséntame TRES textos cortos en [IDIOMA META], uno de nivel BÁSICO, uno INTERMEDIO y uno AVANZADO.
2.  Después de presentarme los TRES textos/escenas, hazme las siguientes preguntas UNA POR UNA para CADA TEXTO/ESCENA, esperando mi respuesta antes de pasar al siguiente.
3.  Finalmente, recomiéndame en qué etapa del Antimétodo (1, 2, 3 o 4) debería enfocarme y dame una breve justificación.

Aquí están las etapas del Antimétodo:
- Etapa 1: Preparación (Vocabulario base).
- Etapa 2: Inmersión Total (Contenido con subtítulos).
- Etapa 3: Free Flow (Contenido sin subtítulos).
- Etapa 4: Producción (Hablar y escribir).

Espera a que te dé mi experiencia previa antes de empezar.`;

function generarYMostrarPrompt() {
  const idiomaMeta = document.getElementById('idiomaMeta').value.trim();
  const experienciaPrevia = document.getElementById('experienciaPrevia').value.trim();
  const promptOutput = document.getElementById('ubicacionPromptToCopy');

  if (!idiomaMeta || !experienciaPrevia) {
    alert("Por favor, completa todos los campos.");
    return;
  }

  let promptPersonalizado = promptPlantilla.replace(/\[IDIOMA META\]/g, idiomaMeta)
                                           .replace('[EXPERIENCIA PREVIA GENERAL]', experienciaPrevia);

  promptOutput.value = promptPersonalizado; 
  document.getElementById('paso2IA').style.display = 'block';
  document.getElementById('paso3Interpreta').style.display = 'block';
  document.getElementById('paso2IA').scrollIntoView({ behavior: 'smooth' });
}

function copyUbicacionPromptToClipboard() { 
  const promptText = document.getElementById('ubicacionPromptToCopy').value;
  const btn = document.getElementById('btnCopiarPrompt');
  const btnText = btn.querySelector('span');

  if (!promptText) return;
  
  navigator.clipboard.writeText(promptText).then(() => {
    const originalText = btnText.innerText;
    btnText.innerText = '¡Copiado con éxito! ✅';
    btn.style.background = '#28a745';
    setTimeout(() => {
      btnText.innerText = originalText;
      btn.style.background = '';
    }, 2000);
  }).catch(() => {
    alert('Error al copiar. Por favor selecciona el texto manualmente.');
  });
}
</script>
