// ./components/NavLink.vue
<script>
export default {
  // Nom du composant (utilisé pour le débogage, n'affecte pas le comportement).
  //doit etre en multi-word (NavLink ou nav-link mais pas navlink)
  name: 'NavLink',

  // Définition des propriétés (props) que ce composant accepte.
  // Ces props sont utilisées pour passer des données au composant depuis l'extérieur.
  props: ['url', 'text']
}
</script>

<template>
  <!-- Modèle du composant qui définit comment il est rendu -->
  <a :href="url">{{ text }}</a>
</template>

<style>
  /* Styles pour le composant NavLink, s'appliquent au lien (a) */
  a {
    text-decoration: none; /* Supprime la décoration de lien (soulignement) */
  }
</style>
