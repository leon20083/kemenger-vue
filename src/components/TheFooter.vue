<template>
  <div class="footer">
    <div class="container">
      <div class="logo">
        <img src="../assets/logo-main.png" alt="" />
      </div>
      <TheMenu />
      <div class="footer-right">
        <img src="../assets/footer-right.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import TheMenu from "./TheMenu.vue";
export default {
  name: "TheFooter",
  components: {
    TheMenu,
  },
};
</script>

<style lang="sass" scoped>
.footer
  background: #0A2530
  padding: 60px 0
  display: flex
  justify-content: space-between
  .logo
    // width: 20%
    img
      // width: 102px
  .footer-right
    width: 20%
    img
      width: 187px
  .top-menu
    width: 50%
    padding: 0
</style>
