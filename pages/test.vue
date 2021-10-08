
<template>
  <div class="wrapper d-flex">
    <div class="mx-auto">
      <v-img :src="require('~/assets/heart.png')"></v-img>
      <p class="test">Jenny</p>
      <p>Jenny</p>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.wrapper {
  background-color: #ade5f7;
  width: 100%;
  height: 937px;
}

.test {
  position: relative;
  bottom: 180px;
  left: 155px;
  color: white;
  font-weight: 900;
  font-family: Helvetica, "Trebuchet MS", Verdana, sans-serif;
}
/* 
.container {
    width: 100%;
    padding: 0px !important;
    margin-right: auto;
    margin-left: auto;
} */
</style>