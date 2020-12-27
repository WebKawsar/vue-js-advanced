<template>
  <div>

    <Header 
    
    :firstName="fname"
    :lastName="lname"
    :age="age"
    @updateName="fname = $event"
    
     />
    <Footer />
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
      age: 25,
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