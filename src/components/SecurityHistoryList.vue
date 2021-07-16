<template>
  <table class="table">
    <tr>
      <th>Action</th>
      <th>IP Address</th>
      <th class="lastth">Time</th>
    </tr>
    <tr bordercolor="red" v-for="user in getUsers" :key="user">
      <td>{{ user.action }}</td>
      <td>{{ user.ip }}</td>
      <td class="lasttd">{{ user.time }}</td>
    </tr>
  </table>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  computed: mapGetters(['getUsers']),
}
</script>

<style lang="scss" scoped>
.table {
  width: 100%;
  border-spacing: 0;
  th {
    text-align: left;
    font-style: normal;
    font-weight: 500;
    font-size: 12px;
    line-height: 140%;
    color: #a3a3a3;
  }
  td {
    padding: 15px 0;
    font-style: normal;
    font-weight: normal;
    font-size: 14px;
    line-height: 17px;
    color: #1d1d1f;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
  }
  .lastth,
  .lasttd {
    text-align: right;
  }
  .lastth {
    padding-right: 70px;
  }
  table td {
    border: 3px solid red;
  }
}
</style>
