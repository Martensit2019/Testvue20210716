<template>
  <div class="sidebar">
    <h1>Sidebar</h1>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.sidebar {
  width: 263px;
  background-color: #9d9d9d;
}
@media (max-width: 600px) {
  .sidebar {
    width: 0;
  }
}
</style>
