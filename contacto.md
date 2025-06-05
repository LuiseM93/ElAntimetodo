---
layout: default
title: Contacto y Comunidad - El Antimétodo
description: Conéctate con el creador del Antimétodo, resuelve tus dudas por Instagram o correo electrónico, y únete a la comunidad de aprendices de idiomas.
---

<style>
.contact-section-card { /* Estilo para la tarjeta de contacto */
  margin-bottom: 3rem; 
  padding: 2.5rem; /* Más padding */
  background-color: var(--card-background); 
  border-radius: 10px; /* Bordes más redondeados */
  box-shadow: 0 5px 15px rgba(0,0,0,0.08); /* Sombra un poco más pronunciada */
  text-align: center;
  border-top: 4px solid var(--primary-color); /* Un acento de color superior */
}
.contact-section-card h2 {
  border-bottom: none; /* Quitar doble borde si ya hay uno en H2 global */
  margin-bottom: 1.5rem; /* Más espacio debajo del H2 */
}
.contact-options-container { /* Contenedor para los botones/links de contacto */
  display: flex;
  flex-direction: column; /* Apilar opciones de contacto */
  align-items: center;
  gap: 1.5rem; /* Espacio entre botón de Instagram y link de email */
  margin: 2rem 0;
}

.email-link-container { /* Contenedor para el texto y el enlace de email */
    margin-top: 1rem;
}

.email-link {
  display: inline-flex; /* Para alinear icono y texto */
  align-items: center;
  font-family: var(--font-primary); /* Fuente principal para destacar */
  font-size: 1.1em; 
  color: var(--secondary-color); 
  font-weight: 500;
  padding: 0.6rem 1rem;
  border-radius: 5px;
  transition: background-color 0.2s ease, color 0.2s ease;
  border: 1px solid var(--light-purple-color); /* Borde sutil */
}
.email-link:hover {
  background-color: var(--light-purple-color);
  color: var(--primary-color);
  text-decoration: none;
}
.email-icon { 
  width: 20px;
  height: 20px;
  vertical-align: middle; 
  margin-right: 8px; 
  fill: currentColor; 
}
</style>

<main class="content-wrapper"> 

  <section style="text-align: center; padding: 2rem 1rem;">
    <h1>Contacto y Comunidad</h1>
    <p class="subtitle" style="font-size: 1.2em; color: var(--secondary-color);">¡Hablemos de idiomas y del Antimétodo!</p>
  </section>

  <section class="contact-section-card">
    <h2>¿Tienes Dudas o Sugerencias?</h2>
    <p style="font-size: 1.1em; margin-top: 1rem; line-height: 1.7; color: var(--text-light-color);">
      Para cualquier consulta sobre El Antimétodo, si necesitas ayuda con algún recurso, o simplemente quieres compartir tu experiencia, las principales formas de contactar son a través de Instagram o correo electrónico:
    </p>
    
    <div class="contact-options-container">
      <a href="https://www.instagram.com/joseluis.hdz.3/" class="btn instagram-link" target="_blank" rel="noopener noreferrer" style="background-color: var(--instagram-color); color: white !important; font-size: 1.1em; padding: 0.8rem 1.8rem;"> <!-- Ajustado padding del botón de Instagram -->
        <svg class="instagram-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" style="width: 22px; height: 22px; margin-right: 8px;">
          <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
        </svg>
        Contactar por Instagram
      </a>

      <div class="email-link-container"> <!-- Contenedor para el texto y el enlace de email -->
        <a href="mailto:joseluishernandeztareas@gmail.com" class="email-link">
          <svg class="email-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 4H4c-1.103 0-2 .897-2 2v12c0 1.103.897 2 2 2h16c1.103 0 2-.897 2-2V6c0-1.103-.897-2-2-2zm0 2l-8 5-8-5h16zm0 12H4V8l8 5 8-5v10z"/></svg>
          joseluishernandeztareas@gmail.com
        </a>
      </div>
    </div>

    <p style="font-size: 1.1em; margin-top: 2.5rem; color: var(--text-light-color);">
      Este sitio web está en constante evolución. ¡Tu feedback es muy valioso para mejorarlo!
    </p>
    
    <!-- Aquí es donde podrías poner la imagen épica de "Supremacía" si decides que va bien en esta página -->
    <!-- <div style="margin-top: 3rem;">
      <img src="{{ '/assets/antimetodo-supremacy-epic.png' | relative_url }}" alt="La Supremacía del Antimétodo es Real" style="max-width: 60%; height: auto; border-radius: 10px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);">
    </div> -->

  </section>

</main>
