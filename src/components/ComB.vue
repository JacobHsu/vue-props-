<template>
    <div>
        <p>ComB : {{fromA}}</p>
    </div>
</template>

<script>
import bus from './bus'

export default {
    name: 'comB',
    data () {
        return {
            fromA: '',
        }
    },
    mounted() {
        bus.$on('fromA', param => {
            this.fromA = param.phone;
        })
    }
}
</script>