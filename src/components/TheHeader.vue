<template>
  <div class="header">
    <p>{{this.page}}</p>
    <button id="headbtn" v-on:click="page = 'account'" >Account</button>
    <button id="headbtn" v-on:click="page = 'voting'" >Voting</button>
    <button id="headbtn" v-on:click="page = 'results'" >Results</button>
    <button id="headbtn" v-on:click="page = 'broardcase'" >Broardcase</button>
  </div>
</template>

<script>
export default {
  name: 'TheHeader',
  props: {
    msg: String
  },
  data: () => ({
    page: 'account',
  }),
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  width: 100%;
  /* margin-top: 60px; */
  background-image: linear-gradient(0deg,  #42b983 0%, #464646 100%);
  color: white;
  position: absolute;
  height: 50px;
  clear:both;
  padding-top:20px;
  top: 0;
  left: 0;
  right: 0;
}
#headbtn {
  background-image: linear-gradient(0deg,  #42b983 0%, #464646 100%);
  width: 25vw;
  height: 50px;

}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
