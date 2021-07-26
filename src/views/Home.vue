<template>
  <div class="home">
    <body id="home-body">
      <h2 class="home-title">Welcome to Coastal Cardano</h2>
  
    </body>
  </div>
</template>

<script> 

export default {
  name: "Home",
  components: {},
};
</script>

<style scoped lang="css">
.home {
  position: relative;
  padding: 1em;
  font-size: 1.25vw;
  height: 100vh;
  margin: -10px;
}

.home::before {
  content: "";
  position: absolute;
  background-image: url(../assets/black_sand_background.jpg);
  background-size: 100%;
  background-repeat: no-repeat;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
  opacity: 0.75;
}

.home-title {
  text-align: center;
  color: white;
}

#home-body {
  margin-top: 10%;
  position: relative;
}
</style>
