<script>
export default {
    data() {
        return {
            showOrHide: false
        };
    },
    methods: {
        toggleElement() {
            this.showOrHide = !this.showOrHide;
        }
    }
};
</script>


<template>
    
    <div class="boolean">
        <button @click="toggleElement"> {{ showOrHide? 'Hide Message' : 'Show Hidden Message'}} </button>
        <div v-if="showOrHide">
            <p> You're seeing me because the condition is true. <br> Or you can hide me again by clicking the button above. </p>
        </div>
        <div v-else></div>              
    </div>
</template>



<style>
.boolean {
    background-color: blanchedalmond;
    text-align: center;
    margin-top: 30px;
    padding: 30px;
}
</style>