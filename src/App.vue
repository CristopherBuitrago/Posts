<template>
    <h1>List of posts:</h1>
    <PostContainer />
    <CounterOption />
    <CounterComposition />
</template>

<script lang="ts" setup>
    import PostContainer from './components/post_component/PostContainer.vue';
    import CounterOption from './components/counter_components/CounterOption.vue';
    import CounterComposition from './components/counter_components/CounterComposition.vue';
</script>

<style>
    body{
        text-align: center;
    }
</style>
