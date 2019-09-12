<template>
  <div class="Children">
    <p>Children Image</p>
    <div class="wrap-img">
        <img :src="imgSrc" :width="imgWidth" :height="imgHeight" :alt="title" @click="doEmit">
    </div>    
  </div>
</template>

<script>
export default {
    name: 'children',
    props:{
        imgWidth: {
            type: Number,
            default: 300
        },
        imgHeight: {
            type: Number
        },
        title: {
            type: String,
            default: ''
        },
        imgSrc: {
            type: String,
            default: ''
        }
    },
    data () {
        return {

        }
    },
    methods: {
        doEmit() {
            const childMsg = '子組件參數xxxx';
            this.$emit('onEmitFunction', childMsg);
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wrap-img{
    text-align: center;
}
</style>
