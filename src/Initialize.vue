<template>
  <div>
    <button @click="init">Init</button>
    <button @click="get">Get</button>
  </div>
</template>

<script>
export default {
  name: 'initializeData',
  methods: {
    init() {
      this.$store.dispath('users/seed')
      this.$store.dispath('conversations/seed')
    }
    get() {
    }
  }
}
</script>

<style lang="css">
</style>
