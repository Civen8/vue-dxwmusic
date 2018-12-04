<template>
  <div>
    <mt-swipe :auto="4000">
      <mt-swipe-item v-for="item in imgList" :key="item.id">
        <img :src="item.img">
      </mt-swipe-item>
    </mt-swipe>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      imgList: [
        { id: 1, img: require('../images/1.jpg') },
        { id: 2, img: require('../images/2.jpg') },
        { id: 3, img: require('../images/3.jpg') }
      ]
    }
  }
}
</script>

<style lang="scss">
.mint-swipe {
  height: 200px;
  overflow: hidden;
  img {
    height: 200px;
  }
}
.mint-swipe-item {
  background-color: red;
}
</style>
