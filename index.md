---
layout: default
title: El Antimétodo - Inicio
description: Aprende idiomas de forma natural con el enfoque del input comprensible. Sin gramática, de forma natural y divertida.
---

<div class="hero-section">
  <div class="hero-content">
    <h1>El Antimétodo</h1>
    <p class="subtitle">Aprende idiomas <strong>sin gramática</strong>, de forma <strong>natural y divertida</strong></p>
  </div>
  <div class="hero-cards-container">
    <div class="hero-card">
      <div class="hero-card-icon">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" width="48px" height="48px"><path d="M12 2C6.486 2 2 6.486 2 12s4.486 10 10 10 10-4.486 10-10S17.514 2 12 2zm0 18c-4.411 0-8-3.589-8-8s3.589-8 8-8 8 3.589 8 8-3.589 8-8 8z"></path><path d="M14.829 14.829a1.994 1.994 0 0 1-2.828 0l-2.414-2.414-2.414 2.414a1.994 1.994 0 0 1-2.828 0L3.172 13.172a1.994 1.994 0 0 1 0-2.828l2.414-2.414-2.414-2.414a1.994 1.994 0 0 1 0-2.828l1.172-1.172a1.994 1.994 0 0 1 2.828 0l2.414 2.414 2.414-2.414a1.994 1.994 0 0 1 2.828 0l1.172 1.172a1.994 1.994 0 0 1 0 2.828l-2.414 2.414 2.414 2.414a1.994 1.994 0 0 1 0 2.828l-1.172 1.172zM9 11.586l-1.293-1.293a.999.999 0 1 0-1.414 1.414L7.586 13l-1.293 1.293a.999.999 0 1 0 1.414 1.414L9 14.414l1.293 1.293a.999.999 0 1 0 1.414-1.414L10.414 13l1.293-1.293a.999.999 0 1 0-1.414-1.414L9 11.586z"></path></svg>
      </div>
      <h2>Sin Estrés</h2>
      <p>Olvida ejercicios aburridos - aprende con contenido que disfrutas.</p>
    </div>
    <div class="hero-card">
      <div class="hero-card-icon">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" width="48px" height="48px"><path d="M12 2C6.486 2 2 6.486 2 12s4.486 10 10 10 10-4.486 10-10S17.514 2 12 2zm0 18c-4.411 0-8-3.589-8-8s3.589-8 8-8 8 3.589 8 8-3.589 8-8 8z"></path><path d="M13 7h-2v5.414l3.293 3.293 1.414-1.414L13 11.586V7z"></path></svg>
      </div>
      <h2>A Tu Ritmo</h2>
      <p>Usa tu tiempo libre: series, música, videojuegos, ¡lo que te guste!</p>
    </div>
  </div>

  <div class="hero-image-container">
    <img src="{{ '/assets/supremacy.jpg' | relative_url }}" alt="Supremacía del Antimétodo" class="hero-main-image">
  </div>
</div>


<style>
.hero-section { 
    text-align: center; 
    padding: 3rem 1rem 2rem 1rem; 
    margin-bottom: 40px; 
    background-color: var(--card-background); 
    border-radius: 12px; /* Más redondeado */
    box-shadow: 0 8px 25px rgba(74, 20, 140, 0.1); /* Sombra morada sutil */
    border: 1px solid var(--light-purple-color); /* Borde muy sutil */
}
.hero-content h1 { 
    font-family: var(--font-primary);
    border-bottom: none; 
    font-size: 3em; /* Un poco más grande */
    margin-bottom: 0.3em; 
    color: var(--primary-color);
    font-weight: 700;
    letter-spacing: -1px; /* Ligeramente más juntas las letras */
}
.hero-content .subtitle { 
    font-family: var(--font-secondary);
    font-size: 1.35em; 
    color: var(--secondary-color); 
    margin-bottom: 2.5rem; 
    font-weight: 400;
}
.hero-cards-container { 
    display: flex; 
    gap: 25px; 
    margin-top: 2rem; 
    justify-content: center; 
    flex-wrap: wrap; /* Para que se adapten en pantallas más pequeñas si es necesario */
}
.hero-card { 
    background: linear-gradient(145deg, var(--card-background), #fdfcff); /* Gradiente sutil */
    padding: 25px 30px; 
    border-radius: 10px; 
    box-shadow: 0 5px 15px rgba(0,0,0,0.07); 
    flex: 1; 
    max-width: 320px; 
    border-top: 4px solid var(--secondary-color); 
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    display: flex;
    flex-direction: column;
    align-items: center; /* Centrar contenido de la tarjeta */
}
.hero-card:hover { 
    transform: translateY(-8px); 
    box-shadow: 0 10px 20px rgba(123, 31, 162, 0.15); /* Sombra morada más pronunciada al hover */
}
.hero-card-icon {
    margin-bottom: 1rem;
    color: var(--secondary-color); /* Color de los iconos SVG */
}
.hero-card-icon svg {
    width: 40px; /* Tamaño de los iconos SVG */
    height: 40px;
}
.hero-card h2 { 
    font-family: var(--font-primary);
    color: var(--primary-color); 
    border-bottom: none; 
    font-size: 1.6em; 
    margin-top: 0; 
    margin-bottom: 0.6rem; 
    font-weight: 600;
}
.hero-card p { 
    font-family: var(--font-secondary);
    font-size: 1em; 
    line-height: 1.6;
    color: var(--text-light-color);
    margin-bottom: 0; /* Quitar margen inferior del párrafo en la card */
}

.hero-image-container {
    margin-top: 2.5rem; /* Espacio sobre la imagen */
}
.hero-main-image {
    max-width: 70%; 
    height: auto; 
    border-radius: 10px; 
    border: 3px solid var(--grey-border-color); 
    box-shadow: 0 6px 18px rgba(0,0,0,0.1); 
}

/* Estilos para secciones generales de contenido, si los necesitas fuera del hero */
.content-section {
  margin-bottom: 3rem;
  padding: 2rem;
  background-color: var(--card-background);
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.05);
}
.content-section .section-title { /* Para H2 dentro de estas secciones */
    text-align: center;
    margin-bottom: 2rem;
}
.content-section .section-subtitle { /* Para un p subtítulo debajo del H2 */
    text-align: center;
    font-size: 1.15em;
    color: var(--text-light-color);
    margin-top: -1.5rem;
    margin-bottom: 2rem;
}

@media (max-width: 768px) {
    .hero-content h1 { font-size: 2.4em; }
    .hero-content .subtitle { font-size: 1.2em; }
    .hero-cards-container { flex-direction: column; gap: 20px; align-items: center;}
    .hero-card { max-width: 90%; } /* Que las tarjetas ocupen más en móvil */
    .hero-main-image { max-width: 90%; }
    .content-section { padding: 1.5rem; }
}
</style>

<!-- CONTENIDO PRINCIPAL (El resto de tu index.md) -->
<main class="content-wrapper"> <!-- Usar la clase global .content-wrapper aquí también -->

  <section class="content-section"> <!-- Ejemplo de cómo usar la nueva clase de sección -->
    <h2 class="section-title">Bienvenido al Antimétodo</h2>
    <p style="font-size: 1.1em; text-align: center; color: var(--text-light-color); line-height: 1.7;"> 
      El Antimétodo es un enfoque revolucionario para aprender idiomas basado en la teoría del <strong>input comprensible</strong>. Olvídate de memorizar reglas gramaticales y ejercicios aburridos. Aquí, aprenderás de manera natural, intuitiva y, sobre todo, ¡disfrutando el proceso!
    </p>
    <p style="font-size: 1.1em; text-align: center; color: var(--text-light-color); line-height: 1.7;"> 
      Sumérgete en contenido real como series, música o videojuegos, y adquiere el idioma como aprendiste tu lengua materna.
    </p>
    <div style="text-align: center; margin-top: 1.5rem;">
      <a href="{{ '/fundamentos' | relative_url }}" class="btn btn-primary">Descubre los Fundamentos</a>
    </div>
  </section>

  <section> <!-- Esta sección no usa .content-section para variar, podrías aplicarlo si quieres fondo blanco -->
    <h2>Beneficios Clave del Antimétodo</h2>
    <ul style="list-style-type: none; padding-left: 0; font-size: 1.1em;">
      <li style="margin-bottom: 1rem; padding: 0.8rem 0.8rem 0.8rem 2.5em; position: relative; background-color: var(--card-background); border-radius: 6px; box-shadow: 0 2px 5px rgba(0,0,0,0.05); border-left: 4px solid var(--secondary-color);">
        <span style="position: absolute; left: 0.8em; top: 50%; transform: translateY(-50%); color: var(--secondary-color); font-weight: bold; font-size:1.2em;">🎯</span> Flexible y personalizado a tus intereses.
      </li>
      <li style="margin-bottom: 1rem; padding: 0.8rem 0.8rem 0.8rem 2.5em; position: relative; background-color: var(--card-background); border-radius: 6px; box-shadow: 0 2px 5px rgba(0,0,0,0.05); border-left: 4px solid var(--secondary-color);">
        <span style="position: absolute; left: 0.8em; top: 50%; transform: translateY(-50%); color: var(--secondary-color); font-weight: bold; font-size:1.2em;">⏱️</span> Aprende con contenido que realmente disfrutas.
      </li>
      <li style="margin-bottom: 1rem; padding: 0.8rem 0.8rem 0.8rem 2.5em; position: relative; background-color: var(--card-background); border-radius: 6px; box-shadow: 0 2px 5px rgba(0,0,0,0.05); border-left: 4px solid var(--secondary-color);">
        <span style="position: absolute; left: 0.8em; top: 50%; transform: translateY(-50%); color: var(--secondary-color); font-weight: bold; font-size:1.2em;">🗣️</span> Desarrolla fluidez natural, sin traducir mentalmente.
      </li>
      <li style="margin-bottom: 1rem; padding: 0.8rem 0.8rem 0.8rem 2.5em; position: relative; background-color: var(--card-background); border-radius: 6px; box-shadow: 0 2px 5px rgba(0,0,0,0.05); border-left: 4px solid var(--secondary-color);">
        <span style="position: absolute; left: 0.8em; top: 50%; transform: translateY(-50%); color: var(--secondary-color); font-weight: bold; font-size:1.2em;">💰</span> Accesible: no necesitas cursos caros, solo contenido e internet.
      </li>
    </ul>
    <div style="text-align: center; margin-top: 2rem;">
      <a href="{{ '/beneficios' | relative_url }}" class="btn">Ver todos los beneficios</a>
    </div>
  </section>

  <section style="margin-bottom: 3rem; text-align: center; padding: 2.5rem 1.5rem; background-image: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%); border-radius: 10px; box-shadow: 0 6px 15px rgba(74, 20, 140, 0.3);">
    <h2 style="color: white; border-bottom: 2px solid rgba(255,255,255,0.5); padding-bottom: 0.5rem; display: inline-block;">¿Listo para Empezar?</h2>
    <p style="font-size: 1.15em; color: var(--light-purple-color); margin-top: 1.5rem; line-height: 1.7;">
      El Antimétodo se estructura en etapas claras para guiarte desde los primeros pasos hasta la fluidez. Cada etapa está diseñada para construir sobre la anterior, asegurando un progreso constante y natural.
    </p>
    <a href="{{ '/etapas' | relative_url }}" class="btn" style="margin-top: 1.5rem; background-color: white; color: var(--primary-color) !important; font-weight: bold;">Explora las Etapas del Antimétodo</a>
  </section>
  
  <section> <!-- Alineación izquierda para estos párrafos -->
     <h2 style="text-align: center;">Próximamente...</h2>
     <p style="text-align: left; color: var(--text-light-color);">Esta es solo la primera versión del sitio web del Antimétodo. Apenas estamos comenzando. La página está en pleno desarrollo y aún faltan muchos recursos, herramientas, ejemplos y guías prácticas que iremos construyendo poco a poco. Lo que acabas de leer es solo el inicio de algo mucho más grande. Se vienen cosas importantes, y esto apenas comienza.</p>
     <p style="text-align: left; color: var(--text-light-color);"><strong>Experiencia del autor:</strong> Gracias al antimétodo, ha logrado avances notables en inglés, francés y alemán. En solo 7 meses y 20 días, alcanzó en francés la etapa 3: entiende casi todo al ver series y películas auténticas sin subtítulos, y juega sus videojuegos favoritos en francés. Todo esto disfrutando el proceso y sintiendo el idioma como una segunda lengua materna. Sin clases ni métodos tradicionales… solo resultados. El antimétodo no es una alternativa —es la supremacía del aprendizaje autodidacta.</p>
     <p style="text-align: left; color: var(--text-light-color);"><strong>Resultados esperados:</strong> fluidez real y un alto nivel en el idioma, comprensión a nivel nativo y hablar desde el instinto.</p>
     <div style="margin-top: 2rem; text-align: center;">
      <img src="{{ '/assets/gato_arquitecto_construccion.jpg' | relative_url }}" 
           alt="Gato arquitecto trabajando en el sitio" 
           style="
             width: 250px;
             border-radius: 12px;
             box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
             border: 3px solid var(--light-purple-color);
           ">
        <p style="font-size:0.85em; color: #777; margin-top: 0.5rem;"><em>Paciencia, estamos construyendo algo genial...</em></p>
    </div>
  </section>

</main>
