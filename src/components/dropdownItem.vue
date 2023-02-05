<script setup lang="ts">



</script>

<template>
    <main>
        <slot name="title"></slot>
        <slot name="items"></slot>
    </main>
</template>

<style>
    main {
        display: flex;
        flex-direction: column;
        background-color: red;
    }

    main div {
        display: none;
        background-color: blue;
    }

    main:hover div {
        display: block;
    }
</style>