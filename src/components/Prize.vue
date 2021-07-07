<template>
  <div id="prize">
    <div class="title">Prize</div>
    <div class="container">
      <div class="box prize">asdf</div>
      <div class="box text">Distinctio non dolorem ratione provident quod dicta distinctio. Repudiandae nesciunt molestiae dolor. Rerum fuga soluta laudantium quia corrupti iste. Officia aut amet necessitatibus sed nihil. Earum non exercitationem blanditiis. Et nesciunt aut rem.

Mollitia harum sed voluptatem modi. Vel facilis repudiandae nam. Minima reiciendis qui et maiores quia atque delectus libero.

Corporis optio saepe nulla. Nostrum natus autem quibusdam laborum. Beatae est quae molestias laborum.</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Prize'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #prize {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin: auto;
    padding: 30px 0;
    background: #000;
  }
  .title {
    flex: 0 0 100%;
    color: #fff;
    font-size: 35px;
  }
  .container {
    max-width: 1100px;
    flex: 0 0 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .box {
    margin: 20px 0;
    flex: 0 0 40%;
    text-align: left;
    background: #333;
  }
  .prize {
    height: 400px;
    width: 400px;
  }
  .text {
    padding: 30px;
    line-height: 1.6em;
    color: #fff;
  }
</style>