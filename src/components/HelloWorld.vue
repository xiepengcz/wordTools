<template>
  <div>
    <div>
      <img class="img" src="../assets/word/高考3500词1.jpg" />
    </div>
    <button class="b-r">默写中文</button>
    <button>默写英文</button>
    <div class="shade">
      <div class="left"></div>
      <div class="center"></div>
      <div class="right"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>
<style land="scss">
.img{
  width: 1000px;
  height: 563px;
}
.b-r{
  margin-right: 20px;
}
.shade{
  .left{}
  .center{}
  .right{}
}
</style>
