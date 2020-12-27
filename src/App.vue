<template>
  <div>

 
    
    {{name}}
    <br>
    {{job}}

    <br>


       <Header />
    <Footer />
  </div>
</template>

<script>
import Header from "./Components/Header/Header";
import Footer from "./Components/Footer/Footer";

export default {
  
  data(){
    return {
      name: "Kawsar Ahmed",
      job: "Learning Web Development"
    }
  },
  components: {
    Header,
    Footer
  }
}
</script>

<style>
  
</style>