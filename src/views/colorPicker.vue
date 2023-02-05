<script lang="ts" setup>
    import dropdownItem from "../components/dropdownItem.vue";
</script>

<template>
    <main>
        <nav>
            <dropdownItem>
                <div class="random">True Random</div>
                <div class="colorTheory">Color Theory</div>
                <div class="shades">Shades</div>
            </dropdownItem>
        </nav>
        <h1 class="title">Color Picker</h1>
    </main>
</template>

<style>
    nav {
        display: flex;
    }
</style>