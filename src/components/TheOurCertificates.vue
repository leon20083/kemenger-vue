<template>
  <div class="certificates" id="certificates">
    <TheTitle title="Наши сертификаты" />
    <img src="../assets/certificates-img.png" alt="" class="img-sert-left" />
    <div class="container">
      <div class="items">
        <ImagesDiv :image="this.imagesSert.one" />
        <ImagesDiv :image="this.imagesSert.two" />
        <ImagesDiv :image="this.imagesSert.three" />
        <ImagesDiv :image="this.imagesSert.four" />
      </div>
    </div>
  </div>
</template>

<script>
import TheTitle from "./TheTitle.vue";
import ImagesDiv from "./ImagesDiv.vue";
export default {
  name: "TheOurCertificates",
  components: {
    TheTitle,
    ImagesDiv,
  },
  data() {
    return {
      // imgUrl: require(this.imagesSert),
      imagesSert: {
        one: require("../assets/sert-1.png"),
        two: require("../assets/sert-2.png"),
        three: require("../assets/sert-3.png"),
        four: require("../assets/sert-4.png"),
      },
    };
  },
};
</script>

<style lang="sass" scoped>
.certificates
  position: relative
  margin-bottom: 100px
  .title
    margin-bottom: 50px
  .img-sert-left
    position: absolute
    left: 0
    top: 30px
    width: 311px
  .items
    display: flex
    justify-content: space-between
    align-items: center
    .img-wrapper
      z-index: 1
      &:not(:last-child)
        margin-right: 15px
</style>
