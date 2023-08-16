<template>
  <div class="maps">
    <div class="container">
      <div class="maps-img-left"></div>
      <div class="maps-img-right"></div>
      <div class="maps-card">
        <img src="../assets/card.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheMaps",
};
</script>

<style lang="sass" scoped>
.maps
  padding-bottom: 90px
  .container
    position: relative
    .maps-card
      width: 795px
      height: 540px
      // border-radius: 20px
      // border: 20px solid #000
      margin: 0 auto
      position: relative
      z-index: 1
      // background: url(<path-to-image>), lightgray -7.716px -2px / 102.322% 100.371% no-repeat
    .maps-img-left
      position: absolute
      top: 60px
      left: 115px
      width: 175px
      height: 175px
      border-radius: 10em
      background: #FFF7BE
      border-left: 25px solid #FAE01A
      border-top: 10px solid #FAE01A
      border-bottom: 10px solid #FAE01A
      z-index: -1
    .maps-img-right
      // @extend .maps-img-left
      position: absolute
      width: 175px
      height: 175px
      bottom: 60px
      right: 115px
      background: #018FA3
      border-radius: 10em
      border: 19px solid #95D8E0
      z-index: -1
</style>
