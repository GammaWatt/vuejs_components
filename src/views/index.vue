<template lang="html">
  <div>
    <image-vue :image="img1_url">
      <div>Attribution</div>
    </image-vue>
  </div>  
</template>

<script>
import Image from '@/components/thing.vue'

export default {
  data () {
    return {
      'img1_url': 'https://drive.google.com/uc?export=view&id=1yIiZKiMcLKSuVBEzcE0od2eCIzI169cy'
    }
  }
  , components: {
    'image-vue': Image
  }
}
</script>

<style lang="css" scoped>
</style>
