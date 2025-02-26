<!-- El archivo App.vue importamos los componentes, de manera que no afecta los cambios de los mismos -->
<template>
  <!-- Escribo la etiqueta Contador, y Vue la reconoce como un componente -->
  <Contador></Contador>
</template>

<script setup>
  // Importamos el archivo Contador.vue, para mostrarlo en la pagina web
  import Contador from './components/Contador.vue';
</script>

<style scoped>
  
</style>
