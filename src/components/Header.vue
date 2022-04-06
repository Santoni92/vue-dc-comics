<template>
  <header>
    <div class="logo">
      <img src="" alt="">
    </div>
    <div class="menu">
      <ul>
        <li v-for="link in links">{{link}}</li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
}
data:{
  links:['CHARACTERS','COMICS','MOVIE']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
  display: flex;
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
