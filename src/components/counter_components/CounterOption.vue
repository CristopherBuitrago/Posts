<!-- 
*  Component made
*  with method
*  Option API
*  Author: @Cristopher-Buitrago
-->

<template>
    <div class="counter-option">
        <h1> Counter With Option API </h1>
        <!-- 
        *  Here Goes the incremented number 
        *  and this can use the methods and data we define below
        -->
        <h3> {{ counter }} </h3>

        <!-- 
        * We define here
        * what we want to do on click
        * in this case we want to use addCounter()
        -->
        <button @click="addCounter()" class="counter-btn">Increment</button>
    </div>
</template>

<!-- 
*  We won't use setup because we want to
*  define and export the component
-->
<script lang="ts">
    // import define component from vue
    import { defineComponent } from 'vue';

    // export this component as default
    export default defineComponent({
        name: 'CounterOption', /* The name of this component */
        components: {}, /* if we use components inside this component we define them here */
        data() { /* We define the data we will use here */
             let counter = 0
             return {counter}
        },
        methods: { /* We put the methods that component have here */
            
            // sum our counter
            addCounter() {
                this.counter++;
            },
            anotherMethod() {
                // another method component have too
            }
        }
    })
</script>

<style scoped>
    .counter-option{
        padding: 10px;
        margin: 5px;
        border-radius: 20px;
        text-align: center;
        background-color: white;
        box-shadow: -5px 5px 20px #111a;
    }

    .counter-btn {
        padding: 15px;
        background-color: blueviolet;
        color: white;
        border: 0;
        outline: 0;
    }

    .counter-btn:hover {
        background-color: white;
        color: blueviolet;
    }
</style>