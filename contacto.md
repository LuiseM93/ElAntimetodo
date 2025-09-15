---
layout: default
title: Sobre Mí - El Antimétodo
description: Conoce a José Luis Hernández, el creador de El Antimétodo. Descubre su historia, su filosofía sobre el aprendizaje de idiomas y cómo contactarlo.
---

<style>
.content-wrapper {
  max-width: 1100px;
}
.about-me-container {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 2.5rem;
  margin-bottom: 4rem;
  background-color: var(--card-background);
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.07);
}
.about-me-image {
  flex: 1;
  min-width: 200px;
  text-align: center;
}
.about-me-image img {
  width: 100%;
  max-width: 250px;
  border-radius: 50%; /* Circular photo */
  box-shadow: 0 8px 20px rgba(0,0,0,0.12);
}
.about-me-text {
  flex: 2;
  min-width: 300px;
}

.contact-section-card {
  max-width: 800px;
  margin: 0 auto 3rem;
  padding: 2.5rem;
  background-color: var(--card-background); 
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.08);
  text-align: center;
  border-top: 4px solid var(--primary-color);
}
.contact-section-card h2 {
  border-bottom: none;
  margin-bottom: 1.5rem;
}
.contact-options-container {
  display: flex;
  justify-content: center; /* Center buttons */
  flex-wrap: wrap; /* Allow wrapping */
  align-items: center;
  gap: 1.5rem;
  margin: 2rem 0;
}

.email-link {
  display: inline-flex;
  align-items: center;
  font-family: var(--font-primary);
  font-size: 1.1em; 
  color: var(--secondary-color); 
  font-weight: 500;
  padding: 0.8rem 1.8rem; /* Match button padding */
  border-radius: 6px; /* Match button radius */
  transition: background-color 0.2s ease, color 0.2s ease;
  border: 1px solid var(--light-purple-color);
  background-color: white;
}
.email-link:hover {
  background-color: var(--light-purple-color);
  color: var(--primary-color);
  text-decoration: none;
}
.email-icon { 
  width: 22px;
  height: 22px;
  vertical-align: middle; 
  margin-right: 8px; 
  fill: currentColor; 
}
</style>

<main class="content-wrapper"> 

  <section style="text-align: center; padding: 1rem 1rem 2rem;">
    <h1>Sobre Mí</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">La historia y filosofía detrás de El Antimétodo</p>
  </section>

  <section class="about-me-container">
    <div class="about-me-image">
      <img src="{{ '/assets/yo.jpg' | relative_url }}" alt="Foto de José Luis Hernández, creador de El Antimétodo">
    </div>
    <div class="about-me-text">
      <h2 style="margin-top:0; font-size: 1.8em;">¡Hola! Soy José Luis</h2>
      <p style="font-size: 1.1em; line-height: 1.7; color: var(--text-light-color);">
        Un joven de 17 años de Tepic, Nayarit.
        <br><br>
        Los idiomas no se estudian, se adquieren. Quien te diga lo contrario te está vendiendo una mentira.
        <br><br>
        Creo firmemente que cualquiera puede adquirir cualquier idioma siempre que aplique la metodología correcta y sea constante. El Antimétodo es la manera científica, natural, divertida, eficiente y flexible de adquirir idiomas. No es marketing, es la verdad.
        <br><br>
        Yo partí desde cero con el francés, no sabía ni lo más básico. Mi proceso fue... "único" e "irrepetible". Recuerdo llegar a mi casa y ponerme a jugar Cyberpunk 2077 para disfrutar al máximo su doblaje en francés. Recuerdo el momento en que más disfruté viendo Hajime no Ippo o Neon Genesis Evangelion sin subtítulos. Fue, como lo dije, "único" e "irrepetible", adquiriendo el idioma de la manera más eficaz, natural y divertida posible.
        <br><br>
        Y por supuesto, cada día utilizo mi app de El Antimétodo y mi filosofía para continuar mi propio viaje con los idiomas.
        <br><br>
        Tú también lo puedes lograr. ¡Solo tienes que intentarlo!
      </p>
    </div>
  </section>

  <section class="contact-section-card">
    <h2>¿Quieres Contactarme o Unirte a la Comunidad?</h2>
    <p style="font-size: 1.1em; margin-top: 1rem; line-height: 1.7; color: var(--text-light-color);">
      Para cualquier consulta, sugerencia, o para unirte a la conversación, estas son las mejores vías:
    </p>
    
    <div class="contact-options-container">
      <a href="https://www.instagram.com/joseluis.hdz.3/" class="btn" target="_blank" rel="noopener noreferrer" style="background-color: var(--instagram-color); color: white !important; font-size: 1.1em;">
        <svg class="instagram-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" style="width: 22px; height: 22px; margin-right: 8px; vertical-align: middle;"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/></svg>
        Instagram del Creador
      </a>
      <a href="https://www.facebook.com/people/El-Antimétodo/61579943335092" class="btn" target="_blank" rel="noopener noreferrer" style="background-color: var(--facebook-color); color: white !important; font-size: 1.1em;">
        <svg class="facebook-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" style="width: 22px; height: 22px; margin-right: 8px; vertical-align: middle;"><path d="M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z"/></svg>
        Facebook de El Antimétodo
      </a>
      <a href="mailto:joseluishernandeztareas@gmail.com" class="email-link">
        <svg class="email-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 4H4c-1.103 0-2 .897-2 2v12c0 1.103.897 2 2 2h16c1.103 0 2-.897 2-2V6c0-1.103-.897-2-2-2zm0 2l-8 5-8-5h16zm0 12H4V8l8 5 8-5v10z"/></svg>
        Correo Electrónico
      </a>
    </div>
  </section>

</main>