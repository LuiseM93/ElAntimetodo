---
layout: default
title: El Antimétodo - Inicio
description: Aprende idiomas de forma natural con el enfoque del input comprensible. Sin gramática, de forma natural y divertida.
---

<div class="hero">
  <h1>El Antimétodo</h1>
  <p class="subtitle">Aprende idiomas <strong>sin gramática</strong>, de forma <strong>natural y divertida</strong></p>
  <div class="hero-cards">
    <div class="card">
      <h2>🎯 Sin Estrés</h2>
      <p>Olvida ejercicios aburridos - aprende con contenido que disfrutas</p>
    </div>
    <div class="card">
      <h2>⏱️ A Tu Ritmo</h2>
      <p>Usa tu tiempo libre: series, música, videojuegos</p>
    </div>
  </div>
</div>

<style>
/* Estos estilos son específicos para el Hero Section de esta página */
.hero {
  text-align: center;
  padding: 2rem 1rem; /* Añadido padding vertical */
  margin-bottom: 40px; /* Esto es del original, se puede ajustar */
  background-color: var(--card-background); /* Fondo blanco para el hero */
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}
.hero h1 {
    border-bottom: none; /* Quitar borde inferior del H1 dentro de hero */
    font-size: 2.8em; /* Hacer el H1 más grande */
    margin-bottom: 0.5rem;
}
.subtitle {
  font-size: 1.3em; /* Ligeramente más grande */
  color: var(--secondary-color);
  margin-bottom: 2rem; /* Más espacio antes de las cards */
}
.hero-cards {
  display: flex;
  gap: 20px;
  margin-top: 30px;
  justify-content: center; /* Centrar las tarjetas si no ocupan todo el ancho */
}
.card {
  background: var(--card-background);
  padding: 25px; /* Más padding */
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.1);
  flex: 1;
  max-width: 300px; /* Limitar ancho máximo de las cards */
  border-top: 4px solid var(--secondary-color); /* Detalle de color */
}
.card h2 {
    color: var(--primary-color);
    border-bottom: none; /* Quitar borde de H2 en cards */
    font-size: 1.5em;
    margin-top: 0;
    margin-bottom: 0.75rem;
}
.card p {
    font-size: 1em;
    line-height: 1.5;
}
.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15); /* Mejorar sombra en hover */
  transition: all 0.3s ease;
}
</style>

<!-- CONTENIDO PRINCIPAL -->
<main style="max-width: 800px; margin: 40px auto 0 auto; padding: 0 1rem;">

  <section style="margin-bottom: 3rem; text-align: center; padding: 2rem; background-color: var(--card-background); border-radius: 8px; box-shadow: 0 3px 10px rgba(0,0,0,0.05);">
    <h2 style="color: var(--primary-color); border-bottom: 2px solid var(--light-purple-color); padding-bottom: 0.5rem; display: inline-block;">Bienvenido al Antimétodo</h2>
    <p style="font-size: 1.1em; margin-top: 1rem;">
      El Antimétodo es un enfoque revolucionario para aprender idiomas basado en la teoría del <strong>input comprensible</strong>. Olvídate de memorizar reglas gramaticales y ejercicios aburridos. Aquí, aprenderás de manera natural, intuitiva y, sobre todo, ¡disfrutando el proceso!
    </p>
    <p style="font-size: 1.1em;">
      Sumérgete en contenido real como series, música o videojuegos, y adquiere el idioma como aprendiste tu lengua materna.
    </p>
    <a href="{{ '/fundamentos' | relative_url }}" class="btn" style="margin-top: 1.5rem; background-color: var(--primary-color);">Descubre los Fundamentos</a>
  </section>

  <section style="margin-bottom: 3rem;">
    <h2 style="color: var(--primary-color); border-bottom: 2px solid var(--light-purple-color); padding-bottom: 0.5rem;">Beneficios Clave del Antimétodo</h2>
    <ul style="list-style-type: none; padding-left: 0; font-size: 1.1em;">
      <li style="margin-bottom: 0.75rem; padding-left: 1.5em; position: relative;">
        <span style="position: absolute; left: 0; color: var(--secondary-color); font-weight: bold;">✔</span> Flexible y personalizado a tus intereses.
      </li>
      <li style="margin-bottom: 0.75rem; padding-left: 1.5em; position: relative;">
        <span style="position: absolute; left: 0; color: var(--secondary-color); font-weight: bold;">✔</span> Aprende con contenido que realmente disfrutas.
      </li>
      <li style="margin-bottom: 0.75rem; padding-left: 1.5em; position: relative;">
        <span style="position: absolute; left: 0; color: var(--secondary-color); font-weight: bold;">✔</span> Desarrolla fluidez natural, sin traducir mentalmente.
      </li>
      <li style="margin-bottom: 0.75rem; padding-left: 1.5em; position: relative;">
        <span style="position: absolute; left: 0; color: var(--secondary-color); font-weight: bold;">✔</span> Accesible: no necesitas cursos caros, solo contenido e internet.
      </li>
    </ul>
    <div style="text-align: center; margin-top: 2rem;">
      <a href="{{ '/beneficios' | relative_url }}" class="btn">Ver todos los beneficios</a>
    </div>
  </section>

  <section style="margin-bottom: 3rem; text-align: center; padding: 2rem; background-color: var(--light-purple-color); border-radius: 8px;">
    <h2 style="color: var(--primary-color); border-bottom: 2px solid var(--primary-color); padding-bottom: 0.5rem; display: inline-block;">¿Listo para Empezar?</h2>
    <p style="font-size: 1.1em; color: var(--text-color); margin-top: 1rem;">
      El Antimétodo se estructura en etapas claras para guiarte desde los primeros pasos hasta la fluidez. Cada etapa está diseñada para construir sobre la anterior, asegurando un progreso constante y natural.
    </p>
    <a href="{{ '/etapas' | relative_url }}" class="btn" style="margin-top: 1.5rem; background-color: var(--primary-color); color: white !important;">Explora las Etapas del Antimétodo</a>
  </section>
  
  <section style="margin-bottom: 3rem; text-align: center;">
     <h2 style="color: var(--primary-color); border-bottom: 2px solid var(--light-purple-color); padding-bottom: 0.5rem;">Próximamente...</h2>
     <p>Esta es solo la primera versión del sitio web del Antimétodo. Apenas estamos comenzando. La página está en pleno desarrollo y aún faltan muchos recursos, herramientas, ejemplos y guías prácticas que iremos construyendo poco a poco. Lo que acabas de leer es solo el inicio de algo mucho más grande. Se vienen cosas importantes, y esto apenas comienza.</p>
     <p><strong>Experiencia del autor:</strong> Gracias al antimétodo, ha logrado avances notables en inglés, francés y alemán. En solo 7 meses y 20 días, alcanzó en francés la etapa 3: entiende casi todo al ver series y películas auténticas sin subtítulos, y juega sus videojuegos favoritos en francés. Todo esto disfrutando el proceso y sintiendo el idioma como una segunda lengua materna. Sin clases ni métodos tradicionales… solo resultados. El antimétodo no es una alternativa —es la supremacía del aprendizaje autodidacta.</p>
     <p><strong>Resultados esperados:</strong> fluidez real y un alto nivel en el idioma, comprensión a nivel nativo y hablar desde el instinto.</p>
     <div style="margin-top: 2rem; text-align: center;">
      <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" 
           alt="Gato arquitecto trabajando en el sitio" 
           style="
             width: 250px; /* Ajustado para que no sea tan grande */
             border-radius: 12px;
             box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
             border: 3px solid var(--light-purple-color);
           ">
        <p style="font-size:0.8em; color: #777;"><em>Paciencia, estamos construyendo algo genial...</em></p>
    </div>
  </section>

</main>
