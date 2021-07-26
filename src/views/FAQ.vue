<template>
  <div class="faq">
   
  </div>
</template>

<script>
export default {
  name: "FAQ",
  head: {
    // creates a title tag in header.
    title() {
      return {
        inner: this.title,
      };
    },
    meta: [
      // creates a meta description tag in header.
      { name: "FAQ", content: "FAQ for Coastal Cardano, Cardano, and ADA" },
    ]
  }
};
</script>

<style scoped lang="css">
.faq {
  align-items: start;
  text-align: left;
  word-break: normal;
  padding-left: 1em;
  font-size: 1.25vw;
}
</style>