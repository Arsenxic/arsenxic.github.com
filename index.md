<style>
/* Animation pour effacer le prénom */
#prenom {
  font-size: 2.5em;
  font-weight: bold;
  text-align: center;
  margin-top: 60px;
  opacity: 1;
  transition: opacity 1s ease;
}
#menu-accueil {
  display: none;
  text-align: center;
  margin-top: 60px;
  font-size: 1.2em;
}
body.prenom-cache #prenom {
  opacity: 0;
}
body.prenom-cache #menu-accueil {
  display: block;
}
</style>
<script>
setTimeout(function() {
  document.body.classList.add('prenom-cache');
}, 2000); // 2 secondes avant disparition du prénom
</script>

<div id="prenom">Arsen</div>
<div id="menu-accueil">
  <a href="#my-projects">Mes Projets</a> |
  <a href="#contact">Contact</a> |
  <a href="https://www.linkedin.com">LinkedIn</a>
</div>


Arsen Aeby

Write a short bio here (who you are, what you do, your interests).

## My Projects
- **Project 1:** Short description of what you did.
- **Project 2:** Short description of another project.

## Contact
- Email: your@email.com
- [LinkedIn](https://www.linkedin.com)

<div style="position: fixed; top: 20px; right: 20px; z-index: 1000;">
  <details>
    <summary style="cursor: pointer; font-weight: bold;">Menu</summary>
    <ul style="list-style: none; padding: 0; margin: 0;">
      <li><a href="#my-projects">Mes Projets</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="https://www.linkedin.com">LinkedIn</a></li>
    </ul>
  </details>
</div>
