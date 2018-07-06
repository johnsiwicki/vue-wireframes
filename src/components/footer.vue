<template>
 <footer class="social-footer">
  <div class="social-footer-left">
    <a href="#"><img class="logo" src="https://placehold.it/150x30"></a>
  </div>
  <div class="social-footer-icons">
    <ul class="menu simple">
      <li><a href="https://www.facebook.com/"><i class="fa fa-facebook" aria-hidden="true"></i></a></li>
      <li><a href="https://www.instagram.com/?hl=en"><i class="fa fa-instagram" aria-hidden="true"></i></a></li>
      <li><a href="https://www.pinterest.com/"><i class="fa fa-pinterest-p" aria-hidden="true"></i></a></li>
      <li><a href="https://twitter.com/?lang=en"><i class="fa fa-twitter" aria-hidden="true"></i></a></li>
    </ul>
  </div>
</footer>
</template>

<script>
  module.exports = {
    props: ["", "", ""],
    data: function() {
      return {
      };
    },
  };
</script>

<style scoped>

.social-footer {
  padding: 1rem;
  background: #8a8a8a;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-align-items: center;
      -ms-flex-align: center;
          align-items: center;
  -webkit-justify-content: space-between;
      -ms-flex-pack: justify;
          justify-content: space-between;
}

.social-footer .social-footer-icons li:last-of-type {
  margin-right: 0;
}

.social-footer .social-footer-icons .fa {
  font-size: 1.3rem;
  color: #fefefe;
}

.social-footer .social-footer-icons .fa:hover {
  color: #4a4a4a;
  transition: color 0.3s ease-in;
}

.menu {
  margin: 0;
  list-style-type: none;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-flex-wrap: nowrap;
      -ms-flex-wrap: nowrap;
          flex-wrap: nowrap;
  -webkit-align-items: center;
      -ms-flex-align: center;
          align-items: center;
  width: 100%;
}

.menu > li {
  -webkit-flex: 0 0 auto;
      -ms-flex: 0 0 auto;
          flex: 0 0 auto;
}

 
.menu > li > a {
  display: block;
  padding: 0.7rem 1rem;
  line-height: 1;
}
</style>
