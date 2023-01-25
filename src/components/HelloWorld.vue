<template>
  <div class="hello">
    <button type="button" style='visibility:hidden'>Click Me!</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
 
  mounted() {
    setTimeout(() => {
            this.$el.querySelector("button").style.visibility = 'visible';
        }, 1500);
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.visible {
  visibility : hidden;
  }
</style>
