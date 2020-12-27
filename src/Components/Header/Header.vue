<template>
    <div>
        Header
        <br>
        <p>{{myName}}</p>
    </div>
</template>

<script>
export default {
    props: {
        myName: {
            type: String,
            required: true
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