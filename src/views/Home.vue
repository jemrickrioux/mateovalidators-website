<template>
    <Header/>
    <div>
      <Validator v-for="node in nodes" :key="node.address" :node="node" />
    </div>
</template>

<script>
import Validator from "@/components/Validator.vue"
import Header from "@/components/Header.vue"

export default {
  name: 'Home',
  components: {Validator, Header},
  props: {
    nodes : {
      type: Array,
      default: () => []
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



</style>
