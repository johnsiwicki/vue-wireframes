<template>
 	<img ref="mainimage" 
    :data-src="src" :class='className' :alt='alt' />
</template>

<script>
  module.exports = {
    props: ["src", "alt", "className"],
    watch: { 
      	src: function(newVal, oldVal) { // watch it
          console.log('Prop changed: ', newVal, ' | was: ', oldVal)
        }
      },
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
