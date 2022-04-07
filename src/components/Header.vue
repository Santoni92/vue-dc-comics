<template>
<div>
 <header>
   <div class="logo">
     <img src="../assets/img/dc-logo.png" alt="">
   </div>
   <div class="menu">
     <ul>
       <li v-for="(item,index) in links" :key="'link-'+index">{{item}}</li>
     </ul>
   </div>
 </header>
</div>
 
</template>

<script>
export default {
  name: 'HeaderComponent',
  props:{
    links:Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
  display: flex;
  justify-content:space-between;
  align-items:center;
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
