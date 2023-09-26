<script lang="ts">
  let Y: number;
</script>

<main>
  <h1>STAR BACARY</h1>
  <video src="/clip.mp4" autoplay muted loop />
  <h1 id="title" class:scrolled={Y > 10}>STAR<br />BACARY</h1>
  <img src="bacary.png" alt="" />
</main>

<svelte:window bind:scrollY={Y} />

<style lang="scss">
  h1 {
    font-family: Libel;
    font-size: 6em;
    margin: 20px;
    text-align: center;
  }
  #title {
    position: absolute;
    right: 81px;
    top: 700px;
    font-size: 9em;
    font-family: Libel;
    line-break: normal;
    .scrolled {
      color: red;
    }
  }
  video {
    width: 100%;
    opacity: 90%;
  }
  img {
    height: 100vh;
    margin-left: 60px;
  }
</style>
