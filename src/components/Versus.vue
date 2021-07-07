<template>
  <div id="versus">
    <div class="container">
      <div class="box team">
        <div class="team-name">TRAINERS OF DOOM</div>
        <div class="team-img"></div>
        <div class="team-vote">VOTE</div>
      </div>
      <div class="box versus-graphic">
        VERSUS
      </div>
      <div class="box team">
        <div class="team-name">TEAM NAKED</div>
        <div class="team-img"></div>
        <div class="team-vote">VOTE</div>
      </div>
    </div>
    <div class="container">
      <div class="hp">
        <div class="hp-1">70%</div>
        <div class="hp-2">30%</div>
      </div>
    </div>
    <div class="container timer">
      <div class="display">{{timeLeft}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Versus',
  data() {
    return {
      timer: 50000
    }
  },
  mounted() {
    setInterval(() => {
      this.timer--
    }, 1000)
  },
  computed: {
    timeLeft() {
      const h =  Math.floor(this.timer / 60 / 60);
      const m = Math.floor(this.timer / 60) - (h * 60);
      const s = this.timer % 60;
      return `${h}h ${m}m ${s}s`;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  #versus {
    margin: 0;
    padding: 30px 0;
    background: #3e25ee;
  }
  .container {
    height: 100%;
    width: 100%;
    max-width: 1100px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .box {
    background: #000;
    padding: 10px;
  }
  .team {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    align-content: space-between;
    width: 500px;
    height: 300px;
    margin: 30px 0 30px 0;
  }
  .team-name {
    margin: -40px 0 0 0;
    z-index: 100;
    background: #000;
    color: #fff;
    padding: 10px 20px;
  }
  .team-img {
    flex: 0 0 100%;
    width: 100%;
    height: 100%;
    background: #333;
  }
  .team-vote {
    padding: 10px 20px;
    margin: -30px 0 0 0;
    font-size: 30px;
    color: #fff;
    background: #000;
  }
  .versus-graphic {
    transform: rotateZ(-4deg);
    background: #cf0080;
    width: 150px;
    margin: 0 -80px;
    padding: 10px 0;
    z-index: 100;
    font-size: 26px;
    color: #fff;
  }
  .hp {
    display: flex;
    justify-content: space-between;
    position: relative;
    height: 50px;
    margin: 0 0px;
    padding: 6px;
    box-sizing: border-box;
    width: 100%;
    max-width: 1100px;
    background:#000;
  }
  .hp div {
    display: flex;
    justify-content: center;
    line-height: 0;
    align-items: center;
    font-size: 34px;
    color: #000;
    height: 100%;
  }
  .hp-1 {
    width: calc(70% - 3px);
    background:#ff00a0;
  }
  .hp-2 {
    width: calc(30% - 3px);
    background: #00f0f0;
  }
  .timer {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .display {
    color: #fff;
    background: #000;
    padding: 2px 20px 10px 20px;
    font-size: 30px;
  }
</style>