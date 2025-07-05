<style>
    @font-face {
  font-family: 'DINdong';
  src: url('fonts/DINdong.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
body, #prenom, #menu-accueil {
  font-family: 'DINdong', Arial, sans-serif;
}
/* Animation pour effacer le prénom */
#prenom {
  font-size: 15em;
  font-weight: bold;
  text-align: center;
  margin-top: 70px;
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
a[href="https://arsenxic.github.io/"] {
  display: none !important;
}
</style>
<script>
setTimeout(function() {
  document.body.classList.add('prenom-cache');
}, 2000); // 2 secondes avant disparition du prénom
</script>

<div id="prenom">Arsen Aeby</div>
<div id="menu-accueil">
  <a href="#my-projects">Mes Projets</a> |
  <a href="#contact">Contact</a> |
  <a href="https://www.linkedin.com">LinkedIn</a>
</div>
