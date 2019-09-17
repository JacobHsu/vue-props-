<template>
    <div>
        ComA: <button @click="sendMsg">给组件B发送消息</button>  
    </div>
</template>

<script>
import bus from './bus'

export default {
    name: 'comA',
    data () {
        return {
            
        }
    },
    
    methods: {
        sendMsg() {
            bus.$emit('fromA', {
                phone: 13800138000
            })
        }
    }
}
</script>