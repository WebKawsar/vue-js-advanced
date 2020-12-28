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

  <BootstrapFrom></BootstrapFrom>

  </div>
</template>

<script>
import compHelper from "./Components/ListHelper/ListHelper";
import BootstrapFrom from "./Components/BootstrapForm/BootstrapForm";

import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

import Vue from 'vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'

// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)


export default {
  
  data(){
    return {
      loader: ""
    }
  },
  components: {
    compHelper,
    BootstrapFrom
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