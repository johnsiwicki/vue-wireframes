<template>
   <video class="video-element" :poster="poster" :controls="controls">
			<source :src="src" type="video/mp4">
   </video>
</template>

<script>
  module.exports = {
		props: ['poster', 'src', 'controls'],
    data: function() {
      return {
 
      }
    }
  }
</script>

<style scoped>

</style>