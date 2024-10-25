<template>
    <div class="post-card">
        <h3>Title</h3>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Autem, reiciendis excepturi laboriosam corrupti sapiente explicabo ratione temporibus qui aliquam impedit ut officia tenetur saepe laborum, labore, incidunt unde aperiam ducimus?</p>
        <PostButton />    
    </div>
</template>

<script lang="ts" setup>
    // IMPORT POST BUTTON
    import PostButton from './PostButton.vue';
</script>

<style scoped>
    .post-card{
        border-radius: 20px;
        padding: 10px;
        margin: 10px;
        border: 1px solid #ccc;
        box-shadow: -5px 5px 20px #111a;
    }
</style>