<template>
  <div class="main">
    <Navbar />
    <SecurityHistory />
    <Navigation />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import SecurityHistory from '@/components/SecurityHistory'
import Navigation from '@/components/Navigation'

export default {
  components: {
    Navbar,
    SecurityHistory,
    Navigation,
  },
}
</script>

<style lang="scss" scoped>
.main {
  width: 100%;
}
</style>
