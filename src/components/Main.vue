<template>
  <main>
      <div class="container">(
        <div class="thumb" v-for="(poster,index) in posters" :key="'poster-' + index">
          <img :src="poster.thumb" :alt="poster.thumb">
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
     display: flex;
    flex-wrap: wrap;
    .thumb{
      width:calc(100% / 6);
    }
  }
</style>