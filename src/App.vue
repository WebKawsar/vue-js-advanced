<template>
  <div>

    {{name}}


    <Header :myName="name" />
    <Footer />
  </div>
</template>

<script>
import Header from "./Components/Header/Header";
import Footer from "./Components/Footer/Footer";

export default {
  
  data(){
    return {
      name: 25,
    }
  },
  components: {
    Header,
    Footer
  }
}
</script>

<style scoped>
  

</style>