<template>
  <div class="CustomMain">
    
    <TopPart/>
    <SecondPart/>
    <ThirdPart/>
    <FourthPart/>

  </div>
</template>

<script>

import TopPart from '../components/TopPart.vue'
import SecondPart from '../components/SecondPart.vue'
import ThirdPart from '../components/ThirdPart.vue'
import FourthPart from '../components/FourthPart.vue'

export default {
  name: 'CustomMain',
  components: {
    TopPart,
    SecondPart,
    ThirdPart,
    FourthPart
  },


  setup() {

    return { }
  }
}
</script>

<style scoped>


</style>
