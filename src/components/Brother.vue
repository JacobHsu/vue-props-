<template>
  <div>
    <comA></comA>
    <comB></comB>
  </div>
</template>

<script>
import ComA from './ComA.vue'
import ComB from './ComB.vue'

export default {
    components: {
       ComA,
       ComB
    },
}
</script>