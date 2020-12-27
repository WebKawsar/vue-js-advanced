<template>
  <div>

    <Header 
    
    :firstName="fname"

     />
    <Footer
    
    :lastName="lname"
  

     />
  </div>
</template>

<script>
import Header from "./Components/Header/Header";
import Footer from "./Components/Footer/Footer";

export default {
  
  data(){
    return {
      fname: "Kawsar",
      lname: "Ahmed",
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