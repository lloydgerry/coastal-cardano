<template>
  <div id="nav" class="nav-bar">
    <div id="nav-left">
      <ul class="nav-item-white">
        <router-link to="/about">About</router-link>
      </ul>
    </div>
    <div id="nav-centre">
      <router-link to="/">
        <h1 class="nav-item-white">Coastal Cardano</h1>
      </router-link>
    </div>
    <div id="nav-right">
      <ul class="nav-item-white">
        <router-link to="/faq">FAQ</router-link>
        |
        <router-link to="/contact">Contact</router-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      isOpen: false,
      active: false,
      navList: [{ url: "#", name: "", children: [] }],
    };
  },
  methods: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="css">
h1 {
  display: block;
  font-size: 2em;
  margin-top: 0.67em;
  margin-bottom: 0.67em;
  margin-left: 0;
  margin-right: 0;
  font-weight: bold;
}

.nav-bar {
  overflow: hidden;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  display: flex;
  justify-content: space-between;
  align-content: center;
  align-items: center;
  background-color: black;
  margin: 0px;
  height: 65px;
  font-size: 120%;
  z-index: 99;

}

#nav {
  padding: 10px 10px; /* Large padding which will shrink on scroll (using JS) */
  transition: 0.4s; /* Adds a transition effect when the padding is decreased */
}
/* style NavBar links when hover */
.nav-bar a:hover {
  color: wheat;
}
/* style NavBar active link  */
.nav-bar a.active {
  color: cyan;
}

.nav-bar .nav-item-white {
  color: white;
  cursor: pointer;
}

.nav-bar #nav-right {
  padding-right: .75em;
}
.nav-bar #nav-left {
  padding-left: .75em;
}
.nav-bar a {
  text-decoration: none;
  color: white;
}
.nav-bar a h1 {
  margin: 1em;
  font-size: 20px;
}
</style>
