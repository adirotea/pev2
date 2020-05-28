<template>
  <div id="app" class="d-flex">
    <pev2 :plan-source="plan" :plan-query="query"></pev2>
  </div>
</template>

<script>
import pev2 from "pev2";

export default {
  name: "App",
  data: function() {
    return {
      plan: this.$route.query.plan || '',
      query: this.$route.query.query || ''
    };
  },
  components: {
    pev2
  }
};
</script>

<style lang="scss">
html,
body,
#app {
  height: 100%;
}
</style>
