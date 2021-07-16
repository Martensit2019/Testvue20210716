<template>
  <div class="navigation">
    <button class="btn btn--blue">Next</button>
    <button class="btn">Previous</button>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.navigation {
  padding: 0 40px;
}
button + button {
  margin-left: 10px;
}
.btn {
  width: 150px;
  height: 42px;
  background-color: transparent;
  border: 1px solid #2469f0;
  border-radius: 30px;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 140%;
  text-align: center;
  color: #2469f0;
  cursor: pointer;
}
.btn--blue {
  background-color: #2469f0;
  color: #fff;
}
</style>
