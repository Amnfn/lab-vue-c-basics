<script>
export default {
    data() {
        return {
            backgroundColor: "",
        };
    },
    methods: {
        changeBackgroundColor() {
            const randomColor = "#" + Math.floor(Math.random() * 16777215).toString(16);
            this.backgroundColor = randomColor;
        },
    },
};
</script>


<template>
    <nav>
        <div :style="{backgroundColor}">
            <button class="footer-button" @click="changeBackgroundColor">Click to change Color</button>
        </div>        
    </nav>
</template>


<style>
.footer-button {
    padding: 10px;
    margin: 5px 0px;
}
</style>