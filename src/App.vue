<template>
  <div>

    <Header :myStudents="students" />
    <Footer />
  </div>
</template>

<script>
import Header from "./Components/Header/Header";
import Footer from "./Components/Footer/Footer";

export default {
  
  data(){
    return {
      students: ["Kawsar", "Shamim", "Imran"]
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