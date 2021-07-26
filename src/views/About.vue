<template>
  <div class="about">
   
  </div>
</template>

<script>
export default {
  name: "About",
  head: {
    // creates a title tag in header.
    title() {
      return {
        inner: this.title,
      };
    },
    meta: [
      // creates a meta description tag in header.
      { name: "About", content: "About Coastal Cardano" },
    ]
  }
};
</script>

<style scoped lang="css">
.about {
  align-items: start;
  text-align: left;
  word-break: normal;
  padding-left: 1em;
  font-size: 1.25vw;
}
</style>
