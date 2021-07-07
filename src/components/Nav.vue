<template>
  <div id="nav">
    <div class="name">
      <span class="nft">NFT</span>rainers
    </div>
    <div class="container navigation">
      <a href="#versus"><div class="link">Versus</div></a>
      <a href="#Teams"><div class="link">Teams</div></a>
      <a href="#tournament"><div class="link">Tournament</div></a>
      <a href="#FAQ"><div class="link">FAQ</div></a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Nav'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #nav {
    max-width: 1100px;
    display: flex;
    justify-content: space-between;
    margin: auto;
    padding: 0px 0;
    background: #000;
  }
  .nft {
    color: red;
  }
  .name {
    font-size: 46px;
    color: #fff;
    font-weight: 900;
    text-transform: uppercase;
  }
  .navigation {
    width: 100;
  }
  a {
    color: #fff;
    text-transform: uppercase;
  }
  .link {
    display: inline-block;
    padding: 20px;
  }
  .link:hover {
    background: #fff;
  }
</style>