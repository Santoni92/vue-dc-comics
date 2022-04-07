<template>
  <div class="card">
      <img :src="contatto.path" :alt="contatto.path">
      <span>{{contatto.text}}</span>
  </div>
</template>

<script>
export default {
    name:'CardContatto',
    props:{
        contatto:Object
    }
}
</script>

<style lang="scss" scoped>
.card{
    display: flex;
}

</style>