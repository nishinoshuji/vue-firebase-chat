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

    }
  }
}
</script>

<style>
</style>
