<template lang="html">
  <div class="div-with-background" :style="style">
    <div>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: [
    "image"
  ]
  , data () {
    return {
      style: {
        backgroundImage: `url(${this.image})`
        , backgroundPosition: 'center'
        , backgroundSize: 'cover'
      }
    }
  }
}
</script>

<style lang="css" scoped>
.div-with-background {
  height: 100px;
  min-width: content;
  min-height: content;
}

.div-with-background > div {
  color: white;
  position: absolute;
  display: block;
  margin: 0 auto;
  bottom: 0;
}
</style>
