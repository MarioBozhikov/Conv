<template>
    <nav class="Nav">
      <img src="~assets/img/logo.png" alt="Logo" class="logo">
      <div class="nav">
      <ul>
        <li><a href="/Link.vue">Home<span></span><span></span><span></span><span></span><span></span></a></li>
        <li><a href="https://Youtube.com" target="_blank">Get A Link!<span></span><span></span><span></span><span></span><span></span></a></li>
        <li><a href="/">Contacts<span></span><span></span><span></span><span></span></a></li>
        <li><a href="/">About<span></span><span></span><span></span><span></span></a></li> 
      </ul>
      </div>
    </nav>
</template>

<script>
    export default {

    }
</script>


<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Russo+One&display=swap");
* {
  font-family: "Russo One", sans-serif;
}

.Nav {
  height: 2em;
  display: flex;
  justify-content: flex-end;
  border-radius: 20em;
  margin: 5px 10px 5px 10px;
  align-items: center;
  padding: 30px 10px 30px 10px;
  background-color: #272932;
  background: linear-gradient(to right, #272932, #475b5a);
}
.logo {
  width: 50px;
  border-left: 120px;
  cursor: pointer;
  margin-right: auto;
}

nav {
  margin: 0;
}
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
}
ul li a {
  --c: #4d7ea8;
  font-weight: bold;
  font-size: 16px;
  color:var(--c);
  border-radius: 5em;
  width: 12em;
  height: 3em;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  text-align: center;
  line-height: 3em;
  position: relative;
  overflow: hidden;
  z-index: 1;
  transition: 0.5s;
  margin: 1em;
  float: left;
  text-decoration: none;
  
}
ul li span { 
  position: absolute;
  width: 25%;
  height: 100%;
  background-color:var(--c);
  background: #f72585;
  transform: translateY(150%);
  border-radius: 50%;
  left: calc((var(--n) - 1) * 25%);
  transition: 0.5s;
  transition-delay: calc((var(--n) - 1) * 0.1s);
  z-index: -1;
}
ul li a:hover {
  color: whitesmoke;
}
ul li a:hover span {
  transform: translateY(0) scale(2);
}
ul li a span:nth-child(1) {
  --n: 1;
}
ul li a span:nth-child(2) {
  --n: 2;
}
ul li a span:nth-child(3) {
  --n: 3;
}
</style>
