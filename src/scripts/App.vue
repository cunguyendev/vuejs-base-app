<template lang="html">
  <table>
    <thead>
      <tr>
        <th>No</th>
        <th>Name</th>
        <th>Class</th>
        <th>Phone</th>
        <th>Address</th>
      </tr>
    </thead>
    <tbody v-for="(user, index) in users" :key="index" class="data-repeat">
      <tr>
        <td>{{ index + 1 }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.class }}</td>
        <td>{{ user.phone }}</td>
        <td>{{ user.address }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script lang="js">
import Vue from 'vue';
import users from './user';

export default Vue.extend({
  data() {
    return {
      bundler: 'Parcel',
      users: users,
    };
  },
});
</script>

<style lang="scss" scoped>
.hello {
  color: green;
}
</style>
