<template>
  <div>
    <app-header       
      :firstName="fName"
      :lastName="lName"
      :id="idd"
      @updateValue="fName= $event">
      </app-header>
    <app-home></app-home>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from "./components/HeaderFile.vue";
import Footer from "./components/FooterFile.vue";
import Home from "./components/HomeFile.vue";

export default {
  name: 'App',
  components: {
    "app-header" : Header,
    "app-footer": Footer,
    "app-home": Home
  },
  data(){
    return{
      fName: "Koyel",
      lName: "das",
      idd: 71
    }
  }
}
</script>
<style>
 body{
  font-family: 'Roboto', sans-serif;
 }
</style>

