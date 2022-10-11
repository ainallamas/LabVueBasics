<template>

    <div class="section">

    <h1 class="title">Iteration 2: Display the result of a Javascript operation in a component's HTML</h1>
    
    <!-- Iteration 2: Using Composition API -->
    <!-- Mensaje: {{message}} <br>
    Suma: {{suma}} 
     -->

    <!-- Iteration 2: Using options API -->
    
    {{property}} <br>
    {{counter}}
    
    </div>

</template>

<script>

// Iteration 2: Using Composition API 

// import { ref } from 'vue'

// const suma = ref(2+2)

// const message = ref (`The sum of 2+2 is: `)


// Iteration 2A: Using Options API

export default {
    data() {
        return{
            counter: 2+2,
            property: 'Blank'
        }
    }, 
    methods: {
        sumar () {
            this.counter;
        }
    },
    created() {
        this.property = 'The sum of 2+2 is:'
    }

}

// Iteration 2B: 











</script>

<style scoped>


</style>