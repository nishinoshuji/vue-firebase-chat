<template>
  <div>
    <button @click="init">Initialize</button>
    <button @click="get">get</button>
  </div>
</template>

<script>
export default {
  name: 'InitializeData',
  methods: {
    init() {
      this.$store.dispatch('users/seed')
      this.$store.dispatch('conversations/seed')
    },
    get() {
      this.$store.dispatch('users/get')
      this.$store.dispatch('conversations/get')
    }
  }
}
</script>

<style>
</style>
