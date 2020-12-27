<template>
    <div>
        Footer
        <br>
        <p>LastName : {{lastName}}</p>
    </div>
</template>

<script>

import { bus } from "../../main";

export default {
  props: {
    lastName: String
  },
  created(){
    bus.$on("changeName", (data) => {
      this.lastName = data;
    })
  }
}
</script>

<style scoped>
  
  div {
    color: rgb(21, 255, 0);
    background-color: blueviolet;
  }
</style>