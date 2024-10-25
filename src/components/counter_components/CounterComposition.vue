<!-- 
 *  Component made
 *  with method
 *  Composition API
 *  when we work with composition
 *  we have major control about
 *  elements reactive
 *  Author: @Cristopher-Buitrago
-->

<template>
    <div class="counter-composition">
        <h1> Counter with composition api</h1>
        <h3> {{ counter }} </h3>
        <button @click="addCounter()" class="counter-btn"> Increment </button>
    </div>
</template>

<script lang="ts" setup>
    // import ref to reference reactive elements
    import { Ref, ref } from 'vue';
           
    /*
     * we define which elements will be reactive with ref
     */
    
    let counter:Ref = ref(0);
    
    const addCounter = ():void => {
        counter.value++;
    }


</script>

<style scoped>
    .counter-composition{
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