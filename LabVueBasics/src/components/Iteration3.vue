<template>

<div class="section">

<h1 class="title">Iteration 3: Show an element only if a particular property is set to true</h1>

<!-- El v-if sirve para hacer condiciones: cuando la condición se cumpla se mostrará en el html. -->
<!-- El v-if, hace desaparecer el elemento del html -->
<div v-if="boolean">Esto es un div en un v-if: se cumple la condición</div>
<div v-else>No se cumple la condición</div>

<!-- A diferencia del v-if el v-show oculta el elemento con un display: none-->
<div v-show="boolean">Esto es un div en un v-show: se cumple la condición</div>

</div>

</template>

<script setup>

import { ref } from 'vue'; 

const boolean = ref(true); 
const show = () => {
    boolean.value = !boolean.value
}


</script>

<style scoped>
</style>