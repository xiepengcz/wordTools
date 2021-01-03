<template>
  <div>
    <div class="img-box">
      <img class="img" src="../assets/word/高考3500词1.jpg" />
      <div class="shade">
        <div class="left" v-show="showLeft"></div>
        <div class="center" v-show="showCenter"></div>
        <div class="right" v-show="showRight"></div>
      </div>
    </div>
    <button class="b-r" @click="dictationCN">默写中文</button>
    <button @click="dictationEN">默写英文</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      count: 0,
      showLeft: true,
      showCenter: false,
      showRight: true
    }
  },
  methods: {
    dictationCN() {
      this.showLeft = false
      this.showRight = true
    },
    dictationEN() {
      this.showLeft = true
      this.showRight = false
    }
  }
}
</script>
<style lang="scss">
.img-box {
  position: relative;
  margin-bottom: 20px;
}
.img {
  width: 1000px;
  height: 563px;
}
.b-r {
  margin-right: 20px;
}
.shade {
  background-color: #fff;
  .left {
    position: absolute;
    top: 0;
    left:242px;
    width: 250px;
    height: 563px;
    background-color: #fff;
  }
  .center {
    position: absolute;
    top: 0;
    left: 490px;
    width: 210px;
    height: 563px;
    background-color: #fff;
  }
  .right {
    position: absolute;
    top: 0;
    left: 704px;
    width: 500px;
    height: 563px;
    background-color: #fff;
  }
}
</style>
