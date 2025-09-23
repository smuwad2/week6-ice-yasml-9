<script>
    export default { 
        // Add Code Here
        data() {
            return {
                message: "Choose your favorite fruit: ",
                fruit1: "apple",
                fruit2: "banana",
                fruit3: "calcium",
                // challenge: use array  
                fruits: ["apple", "banana", "calcium"]
            }
        }
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
    </div>
    <h3>Using Array</h3>
    {{ message }} </br>
    <span v-for="fruit in fruits">
        {{ fruit }} <input type="radio" name="fruit">
    </span>
</template>

<style scoped>
</style>
