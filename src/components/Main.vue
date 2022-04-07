<template>
  <main>
      <div class="container">
        <div class="thumb" v-for="(poster,index) in posters" :key="'poster-' + index">  <!--poster mi rappresenta il singolo oggetto dell'array passato tramite props-->
          <img :src="poster.thumb" :alt="poster.thumb">
          <div class="text">{{poster.series}}</div>
        </div>
      </div>
  </main>
</template>

<script>
export default {
    name:'MainComponent',
    props: {
    posters: Array
}
}
</script>

<style lang="scss" scoped>
  .container{
     max-width: 1200px;
     margin: 0 auto;
     background-color: #1c1c1c;
     display: flex;
    flex-wrap: wrap;
    .thumb{
      width:calc(100% / 6);
      .text{
        color:white;
        font-size:20px;
      }
    }
  }
</style>