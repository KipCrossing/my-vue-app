<template>
  <div class="footer">
    <p>Made by Kippy</p>
  </div>
</template>

<script>
export default {
  name: 'TheFooter',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  width: 100%;
  /* margin-top: 60px; */
  background-image: linear-gradient(0deg, #1f1f1f 0%, #464646 100%);
  color: white;
  position: absolute;
  height: 50px;
  clear:both;
  padding-top:20px;
  bottom: 0;
  left: 0;
  right: 0;
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
