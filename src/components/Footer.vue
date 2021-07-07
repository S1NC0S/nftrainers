<template>
  <div id="footer">
    <div class="socials"></div>
    <div class="socials"></div>
    <div class="socials"></div>
    <div class="socials"></div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #0ff;
    height: 400px;
    margin: 50px 0 0 0;
  }
  .socials {
    background: #000;
    width: 100px;
    height: 100px;
  }
</style>