<template>
  <div class="callout home">
    <h1>Trade or View your Portfolio</h1>
    <h6>You may Save or Load your Data</h6>
    <h6>Click on 'End Day' to begin a new Day!</h6>
    <hr>
    <p>Your Funds: {{ funds | currency }}</p>
  </div>
</template>

<script>
  export default {
    computed: {
      funds() {
        return this.$store.getters.funds;
      }
    }
  }
</script>

<style lang="scss" scoped>
  .home {
    margin-top: 12px;
  }
</style>
