<template>
<div class="grid-container">
  <div class="video">
   <video class="video-element" :poster="poster" :controls="controls">
			<source :src="src" type="video/mp4">
   </video>
  </div>
  <div class="content">

  <h2>This explains the video</h2>
  </div>
</div>
 
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

.grid-container {
  display: grid;
  height: 100%;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;
  grid-template-areas: "video content";
  background:#cacaca;
  margin: 30px 0; 
}

.video {
  grid-area: video;
}

.content {
  grid-area: content;
}


</style>