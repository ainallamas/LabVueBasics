<template>

<div class="section">

<h1 class="title">Iteration 4: Display a list of elements that are stored inside a component </h1>

<div v-for="recipe in italianReceipes ">
    <ItalianReceipes :title="recipe.title" :description="recipe.description" :content="recipe.content" :imagen="recipe.imagen"/>
</div>

</div>

</template>


<script setup>

import ItalianReceipes from './ItalianReceipes.vue'

const italianReceipes = [
{
    title:'Pizza margherita',
    description: 'La madre de todas las pizzas',
    content: '220gr masa de pizza, 90gr queso mozzarella, albahaca fresca, 100gr salsa de tomate',
    imagen: 'https://www.recetasderechupete.com/wp-content/uploads/2017/01/pizza_margarita.jpg'
}, 
{
    title:'Spaghetti alla carbonara',
    description: 'La auténtica salsa carbonara de Italia',
    content: '400gr de espaguetis, 2 huevos, 150gr queso curado, 120gr panceta',
    imagen: 'https://www.recetassinlactosa.com/wp-content/uploads/2015/06/Espaguetis-Carbonara-1.jpg'
}, 
{
    title:'Insalata di burrata',
    description: 'El sabor del sur de Italia',
    content: '1 pieza de burrata, tomate, brotes de rúcula, pesto genovese, albahaca',
    imagen: 'https://images.hola.com/imagenes/cocina/recetas/20210726193661/ensalada-burrata-tomates-albahaca/0-979-276/ensalada-burrata-adob-m.jpg'
}, 

]

</script>

<style scoped>
</style>