<template>
  <header>
      <p>###########[S]AppHeader###########</p>
      <h1>{{ propsdata }}</h1>
      <button v-on:click="sendEvent">send</button>
      <p>###########[E]AppHeader###########</p>
  </header>
</template>

<script>
export default {
    props: ['propsdata'],
    methods: {
        sendEvent: function name() {
            this.$emit('renew')
        }
    }
}
</script>

<style>

</style>