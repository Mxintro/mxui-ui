<template>
  <div id="nav-bar">
    <div class="nav-left"><slot name="left"></slot></div>
    <div class="nav-center"><slot name="center"></slot></div>
    <div class="nav-right"><slot name="right"></slot></div>
  </div>
</template>

<script>
export default {
  name: "MxNavBar",
};
</script>

<style>
#nav-bar {
  position: relative;
  z-index: 10;

  display: flex;

  height: 44px;
  line-height: 44px;
  text-align: center;
}

.nav-left {
  width: 60px;
}

.nav-center {
  flex: 1;
}

.nav-right {
  width: 60px;
}

.nav-left img,
.nav-right img {
  width: 22px;
  height: 22px;
  vertical-align: middle;
}
</style>