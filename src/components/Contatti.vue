<template>
  <div class="dc-contatti">
    <div v-for="contact in contacts" :key="contact">
      <CardContatto :contatto="contact"/>
    </div>
  </div>
</template>

<script>
import CardContatto from '@/components/CardContatto.vue'
export default {
    name: 'ContattiComponent',
    props:{
      contacts:Array
    },
    components:{
      CardContatto
    }
}
</script>

<style lang="scss" scoped>
  .dc-contatti{
    background-color: #0282f9;
    display:flex;
    justify-content:space-between;
    padding:50px 100px;
    color:white;
  }
</style>