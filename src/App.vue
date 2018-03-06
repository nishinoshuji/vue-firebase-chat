<template>
  <div>
    <Initialize />
  </div>
</template>

<script>
import Initialize from './components/Initialize.vue'

export default {
  name: 'app',
  components: {
    Initialize
  },
  created() {
    console.log(this.$store.state.db);
  }
}
</script>

<style>
</style>
