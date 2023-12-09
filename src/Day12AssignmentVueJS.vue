<template>

<h1>Day 12 Assignment Vue js</h1>
<br>
<p class="bold-text">Count: {{ currentCount }}</p>
<br>
<p class="bold-text">Message:{{ theMessage }}</p>
<br>
<button v-on:click="increment()"> Increment </button>
<button v-on:click="decrement()"> Decrement </button>
<br>



</template>

<script>

export default {

    name: "Day12AssignmentVueJS",

    data(){
        return{
            currentCount: 0,
            theMessage:"",
        };
    },

    methods: {

        increment(){

            this.currentCount++;
            this.theMessage = "You have just increment the count";

        },

        decrement(){
            
            this.currentCount--;
            this.theMessage = "You have just decrement the count";

        },
    }
}


</script>

<style scoped>

.bold-text {
    font-weight: bold;
  }

</style>