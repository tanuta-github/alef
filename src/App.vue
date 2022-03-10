<template>
  <div class="wrapper">
    <AppHeader />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
export default {
  name: 'App',
  components: {
    AppHeader
  }
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');

* {
  margin: 0;
  padding: 0;
  font: 12px/1 "Open Sans", sans-serif;
}

.container {
  max-width: 1390px;
  padding: 0 15px;
  margin: 0 auto;
}

</style>
