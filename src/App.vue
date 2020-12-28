<template>
  <div>

    <compHelper>

      <ul slot="listItem">
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
      </ul>
      <p slot="para">Paragraph</p>
      <p :slot="loader">Paragraph</p>
    </compHelper>

  </div>
</template>

<script>
import compHelper from "./Components/ListHelper/ListHelper";

export default {
  
  data(){
    return {
      loader: ""
    }
  },
  components: {
    compHelper
  },
  created(){
    setTimeout(() => {
      this.loader = "other";
    }, 3000)
  }
}
</script>

<style scoped>
  

</style>