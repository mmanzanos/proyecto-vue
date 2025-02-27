<!-- El archivo App.vue importamos los componentes, de manera que no afecta los cambios de los mismos -->
<template>
  <!-- Escribo la etiqueta Contador, y Vue la reconoce como un componente -->
  <MainView></MainView>
</template>

<script setup>
  // Importamos el archivo Contador.vue, para mostrarlo en la pagina web
  import MainView from './views/MainView.vue';
</script>

<style scoped>
  
</style>
