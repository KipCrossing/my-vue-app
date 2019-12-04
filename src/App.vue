<template>
  <div id="app">
    <TheHeader/>
    
    <div class="content-container">
      <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
      <HelloWorld v-if="false" msg="Welcome to Your Vue.js App"/>
      <Registration v-if="comp == 'REGISTRATION'" msg="REGO"/>
    </div>
    <TheFooter/>

  </div>
</template>


<script>
import HelloWorld from './components/HelloWorld.vue'
import TheFooter from './components/TheFooter.vue'
import TheHeader from './components/TheHeader.vue'
import Registration from './components/Registration.vue'


export default {
  name: 'app',
  components: {
    HelloWorld,
    TheFooter,
    TheHeader,
    Registration
  },
  data: () => ({
    comp: 'REGISTRATION',

  }),
}
</script>

<style>
html {
  position: relative;
  min-height: 100%;
}

body {
  margin: 0 !important;
  /*margin-bottom: 300px;*/
  background-color: white;
  min-height: 100%;
}


#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  
  
}

.content-container {
  width: 100vw;
  min-width: 100vw;
  padding-top: 64px;
  padding-bottom: 100px; 
}
</style>
