<template>

<div class="card">

<div class="card-image">
  <figure class="image is-4by3">
      <!-- Ponemos los dos puntos antes de src para decirle que le pasaremos la variable desde el script -->
    <img :src="props.imagen" alt="Placeholder image">
  </figure>
</div>

<div class="card-content">
  <div class="content">
      <div class="card-title">{{props.title}}</div>
      <div>{{props.description}}</div>
      <div>{{props.content}}</div>
  </div>
</div>

</div>


</template>

<script setup>

import { defineProps } from 'vue'

// Definimos los props que vamos a recibir en el componente
const props = defineProps (['title', 'description', 'content', 'imagen']); 


</script>

<style scoped>
</style>