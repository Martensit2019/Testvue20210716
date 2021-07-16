<template>
  <div class="app">
    <div class="container">
      <div class="app__wrapper">
        <Sidebar />
        <Main />
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from '@/components/Sidebar'
import Main from '@/components/Main'

export default {
  components: {
    Sidebar,
    Main,
  },
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  min-height: 100%;
  font-family: Montserrat;
}
.app__wrapper {
  display: flex;
}
.container {
  max-width: 1440px;
  padding: 0 15px;
  margin: 0 auto;
}
</style>
