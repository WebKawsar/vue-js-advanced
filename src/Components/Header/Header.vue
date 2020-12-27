<template>
    <div>
        Header
        <br>


        <p>{{firstName}}</p>
        <p>{{lastName}}</p>
        <p>{{age}}</p>

        <button @click="updateName">Update yor name</button>
    </div>
</template>

<script>
export default {
    props: {
        firstName: String,
        lastName: String,
        age: Number
    },
    methods: {
        updateName(){
            // this.firstName = "Abdullah"
            this.$emit("updateName", "Abdullah");
        }
    }
}
</script>


<style scoped>
  
  div {
    color: green;
    background-color: aqua;
  }
</style>