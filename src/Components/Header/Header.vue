<template>
    <div>
        Header
        <br>


        <p>Firstname : {{firstName}}</p>
        
        <button @click="updateName">Update yor name</button>
    </div>
</template>

<script>

import { bus } from "../../main";

export default {
    props: {
        firstName: String,
    },
    methods: {
        updateName(){
            bus.$emit("changeName", "Ahmed changed to Mohammad")
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