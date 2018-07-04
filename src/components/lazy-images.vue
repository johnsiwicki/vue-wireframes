<template>
 	<img ref="mainimage" 
    :data-src="src" :class='className' :alt='alt' />
</template>

<script>
  module.exports = {
    props: ["src", "alt", "className", "finalImage"],
    data: function() {
      return {
      };
    },
  mounted() {
      var imgy = this.src;
      let mainImage = this.$refs.mainimage;
      mainImage.src = imgy;
  },

  };
</script>

<style scoped>

</style>
