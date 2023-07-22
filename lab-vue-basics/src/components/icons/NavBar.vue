<script setup>
const navbar = ["Account", "Home", "Shop", "Service Center"]
</script>

<template>
    <nav class="navbar">
        <ul class="nav-list">
            <li v-for="nav in navbar">
                {{ nav }}
            </li>
        </ul>
    </nav>
</template>

<style>
.nav-list {
    list-style-type: none;
    display: flex;
    justify-content: space-around;
}

</style>