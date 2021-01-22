<template lang="html">
  <p class="hello">Hello {{ bundler }}</p>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  data() {
    return {
      bundler: 'Parcel',
    };
  },
});
</script>

<style lang="scss" scoped>
.hello {
  color: green;
}
</style>
