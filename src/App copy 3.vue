

<script>
import userData from '/home/roy/S2P/demoproj/src/dp.json'

export default {
  data() {
    return {
      users: userData,
    };
  },
};
</script>

<template>
  <p v-for="user in users" :key="user.name">
      {{user.name}}
      {{user.successRate}}
  </p>
</template>

