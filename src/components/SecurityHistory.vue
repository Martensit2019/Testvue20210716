<template>
  <div class="securityhistory">
    <div class="securityhistory__top">
      <div class="securityhistory__title">Security history</div>
      <div class="securityhistory__icons">
        <img src="../assets/icons/icon-1.svg" alt="" />
        <img src="../assets/icons/icon-2.svg" alt="" />
      </div>
    </div>
    <SecurityHistoryList />
  </div>
</template>

<script>
import SecurityHistoryList from '@/components/SecurityHistoryList'

export default {
  components: { SecurityHistoryList },
}
</script>

<style lang="scss" scoped>
.securityhistory {
  padding: 0 40px 65px;
  &__top {
    display: flex;
    margin-bottom: 20px;

    justify-content: space-between;
    align-items: center;
  }
  &__title {
    font-family: Montserrat;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 24px;
    color: #000000;
  }
  &__icons {
    display: flex;
    align-items: center;
    img {
      width: 34px;
      height: 34px;
      cursor: pointer;
      & + img {
        margin-left: 5px;
      }
    }
  }
}
</style>
