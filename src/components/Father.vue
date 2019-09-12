<template>
  <div class="father">
    <p>點擊圖片</p>
    <hw-child :img-src="imgSrc" :img-width="300" :img-height="imgHeight" title="靜態文字" @onEmitFunction="emitFuction"></hw-child>
    <h2><a href="http://www.helloweba.net/javascript/612.html">Vue組件間通信：父子組件通信</a></h2>
  </div>
</template>

<script>
import Children from './Children.vue'
export default {
  name: 'Father',
  components: {
    hwChild: Children,
  },
  data() {
    return {
        imgHeight: 300,
        imgHeight: 300,
        imgSrc: 'https://cli.vuejs.org/favicon.png'
    }
  },
  methods: {
    emitFuction(val) {
        console.log(val);
        alert('獲取子組件參數：'+ val);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
