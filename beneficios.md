---
layout: default
title: Beneficios del Antimétodo
description: Descubre las ventajas de aprender idiomas con el Antimétodo, como la flexibilidad, el aprendizaje natural y la accesibilidad.
---

<main style="max-width: 800px; margin: 0 auto; padding: 0 1rem;">

  <section style="margin-bottom: 3rem;">
    <h1>Beneficios del Antimétodo</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">Más que un método, una forma natural y efectiva de adquirir idiomas.</p>
    
    <div style="
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); /* Ajustado minmax para mejor responsiveness */
      gap: 1.5rem;
      margin: 2rem 0;
    ">
      <div class="benefit-card">
        <h3>Flexible y personalizado</h3>
        <p>Se adapta a cada estudiante según sus intereses, nivel y ritmo.</p>
      </div>
      
      <div class="benefit-card">
        <h3>Aprovecha tu tiempo</h3>
        <p>Sustituye tiempo en redes sociales por aprendizaje placentero.</p>
      </div>
      
      <div class="benefit-card">
        <h3>Fluidez natural</h3>
        <p>Habla sin traducir, con un "instinto" similar al nativo.</p>
      </div>
      
      <div class="benefit-card">
        <h3>Accesible</h3>
        <p>No requiere pagar cursos caros, solo internet y contenido.</p>
      </div>
      
      <div class="benefit-card">
        <h3>Hábitos sostenibles</h3>
        <p>Construye disciplina sin depender de motivación.</p>
      </div>
      
      <div class="benefit-card">
        <h3>Etapas claras</h3>
        <p>Proceso bien definido y fácil de seguir.</p>
      </div>
      
      <div class="benefit-card">
        <h3>Autoaprendizaje real</h3>
        <p>Capacidad de aprender cualquier idioma por ti mismo.</p>
      </div>
    </div>
    
    <div style="text-align: center; margin: 3rem 0;">
      <img src="{{ '/assets/welearnthisway.png' | relative_url }}" alt="We Learn This Way - El Antimétodo"
           style="
             max-width: 50%;
             height: auto;
             border: 3px solid var(--light-purple-color);
             border-radius: 8px;
             box-shadow: 0 4px 10px rgba(74, 20, 140, 0.2);
           ">
    </div>
  </section>

</main>

<style>
  .benefit-card {
    background: var(--card-background);
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    border-left: 4px solid var(--secondary-color); /* Detalle de color */
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  .benefit-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 15px rgba(0,0,0,0.15);
  }
  .benefit-card h3 {
    color: var(--primary-color); /* Títulos de tarjeta con color primario */
    margin-top: 0;
    margin-bottom: 0.5rem;
    border-bottom: none; /* Sin borde inferior para H3 en tarjetas */
  }
</style>
