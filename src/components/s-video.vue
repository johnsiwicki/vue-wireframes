<template>
<div class="grid-container">
  <div class="video">
   <video class="video-element" :poster="poster" :controls="controls">
			<source :src="src" type="video/mp4">
   </video>
  </div>
  <div class="content">

  <h2>This explains the video</h2>

     <p>Cupcake cotton candy gingerbread pie lollipop. Tootsie roll sugar plum tootsie roll jelly beans jelly chocolate bar.</p>
     <p>Tiramisu cupcake tiramisu cookie candy canes dragée apple pie. Tiramisu cupcake tiramisu cookie candy canes dragée apple pie.</p>

      <button>Let's Do It</button>
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
  background:#3C444C;
  margin: 30px 0; 
}

.video {
  grid-area: video;
}

.content {
  grid-area: content;
  color:white;
  padding: 0 15px;
}


</style>