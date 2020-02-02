<template>
  <div class="logo-wrapper navbar-item">
    Aituglo
  </div>
</template>
<script>
export default {
  name: 'SiteLogo'
}
</script>
<style lang="scss">
@keyframes logoBlink {
  100% {
    transform: translateY(-360px);
  }
}
.logo-wrapper {
  position: relative;
  height: 50px;
  overflow: hidden;
  width: 200px;
}
</style>
