<script setup>
const navbar = ["Math Operation", "Boolean Variable", "Displaying elements", "Bonus"]
</script>

<template>
    <nav class="navbar">
        <h2></h2>
        <ul class="nav-list">
            <li v-for="nav in navbar">
                {{ nav }}
            </li>
        </ul>
    </nav>
</template>

<style>
.navbar {
    color: blue;
    font-weight: 400;
}
.nav-list {
    list-style-type: none;
    display: flex;
    justify-content: space-around;
}

</style>