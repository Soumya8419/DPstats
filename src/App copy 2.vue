<template>
  <p v-for="user in users" :key="user.id">
    {{user.id}}
      {{user.name}}
  </p>
</template>

<script>
import userData from '/home/roy/S2P/demoproj/src/users.json'

export default {
  data() {
    return {
      users: userData,
    };
  },
};
</script>

