<template>
<nav>
  <input type="checkbox" id="checkbox1" />
  <label for="checkbox1">
<ul class="menu first">
  <li><a href="#">HOME</a></li>
  <li><a href="#">ABOUT</a></li>  
  <li><a href="#">CONTACT</a></li>  
  <li><a href="#">FAQS</a></li>  
</ul>
  <span class="toggle">☰</span>
  </label>
</nav>
</template>

<script>
module.exports = {
  data: function() {
    return {};
  }
};
</script>

<style scoped>
nav {
  margin: 50px auto;
  max-width: 100%;
  width: 100%;
  font-family: "Droid Sans", sans-serif;
}

#checkbox1,
#checkbox2,
#checkbox3,
.toggle {
  display: none;
}

.menu {
  padding: 0;
  margin: 0;
  max-width: 100%;
  height: 50px;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  list-style-type: none;
}

.menu li a {
  text-decoration: none;
  align-self: center;
  font-size: 14px;
  padding: 16px 20px;
  transition: background 0.2s linear;
}

@media screen and (max-width: 600px) {
  .menu li a {
    font-size: 13px;
  }
}

@media screen and (max-width: 550px) {
  .toggle {
    clear: both;
    display: block;
    text-align: center;
    font-size: 14px;
    line-height: 40px;
    cursor: pointer;
    width: 100%;
    height: 40px;
    font-size: 18px;
    color: #595959;
    background: #dbdbdb;
    transition: all 0.1s linear;
  }
  .toggle:hover {
    background: #cecece;
  }
  #checkbox1:checked + label .first li {
    opacity: 1;
    visibility: visible;
    transition: all 0.7s linear;
  }
  #checkbox2:checked + label .second li {
    opacity: 1;
    visibility: visible;
    transition: all 0.7s linear;
  }
  #checkbox3:checked + label .third li {
    opacity: 1;
    visibility: visible;
    transition: all 0.7s linear;
  }
  #checkbox1:checked + label .first {
    height: 200px;
  }
  #checkbox2:checked + label .second {
    height: 200px;
  }
  #checkbox3:checked + label .third {
    height: 200px;
  }
  .menu {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    height: 0px;
    transition: height 0.3s linear;
  }
  .menu li {
    display: flex;
    /* magic */
    align-self: center;
    width: 100%;
    opacity: 0;
    visibility: hidden;
  }
  .menu li a {
    width: 100%;
    text-align: center;
    align-self: center;
    align-content: center;
  }
}

.first {
  background: #625b60;
}

.first li a {
  color: #fff;
}

.first li a:hover {
  background: #6d6268;
}

.second {
  background: #51535f;
}

.second li a {
  color: #fff;
}

.second li a:hover {
  background: #5d5f6d;
}

.third {
  background: #eee;
}

.third li a {
  color: #606060;
}

.third li a:hover {
  background: #d5d5d5;
}

body {
  background: #fff;
}
</style>
