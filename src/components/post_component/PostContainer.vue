<template>
    <div class="post-container">
        <PostCard />
        <PostCard />
        <PostCard />
        <PostCard />
    </div>
</template>

<script lang="ts" setup>
    import PostCard from './PostCard.vue';
</script>

<style scoped>
    .post-container{
        justify-content: center;
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }
</style>