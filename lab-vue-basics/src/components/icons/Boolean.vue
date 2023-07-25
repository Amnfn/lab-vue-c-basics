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
        <div v-if="showOrHide">
             You're seeing me because the condition is true. <br> Or you can hide me again by clicking the button below.
        </div> 
        <div v-else> I have a message for you! Click me! </div> 
        <button @click="toggleElement"> {{ showOrHide? 'Hide Message' : 'Show Hidden Message'}} </button>             
    </div>
</template>



<style>
.boolean {
    background-color: blanchedalmond;
    text-align: center;
    margin-top: 30px;
    padding: 30px;
}
div {
    margin-bottom: 20px;
}
</style>