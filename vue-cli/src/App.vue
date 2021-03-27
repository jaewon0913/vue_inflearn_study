<template>
  <div>
    {{ str }}
    <app-header 
    v-bind:propsdata="appHeaderStr"
    v-on:renew="renewStr"></app-header>
  </div>
  <!--
  ROOT 아래에는 하나의 element만 들어갈 수 있다.
  <div></div>
  -->
</template>

<script>
import AppHeader from './components/AppHeader.vue';

export default {
  data: function name() {
    return {
      str: 'hi',
      appHeaderStr: 'Test App Header String'
    } 
  },
  components: {
    'app-header' : AppHeader
  },
  methods: {
    renewStr: function name() {
      this.appHeaderStr = 'Hello Vue'
    }
  }
}
</script>

<style>

</style>