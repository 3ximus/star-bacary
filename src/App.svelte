<script lang="ts">
  let Y: number;
</script>

<main>
  <h1 id="header" class:scrolled={Y > 20}>STAR BACARY</h1>
  <p class="spacer"></p>
  
  <video src="/clip.mp4" autoplay muted loop />
  <h1 id="title">STAR<br />BACARY</h1>
  <img src="bacary.png" alt="" />
  <p>
    Avec sa maîtrise parfaite du rythme africain du 21e siècle, à la frontière
    du mystique, Star Bacary est résolument tourné vers le monde. Bacary né
    Sonko est originaire du département de Goudomp, près de Ziguinchor, là où
    coulent les murmures du fleuve Casamance. Très tôt conscientisé aux maux de
    la société africaine dont le sort incertain de la jeunesse, il ouvre grand
    les yeux sur les déroutes des politiciens à l'égard de sa génération. Il
    devient leur porte-voix, d'ouest en est de sa Casamance, et à travers la
    diaspora. Le destin tragique de ses amis exilés dans de fatales « pirogues
    cercueils » le pousse à écrire sa première chanson en 2012, à l'âge de 19
    ans "Immigration clandestine"/"Toukou toukou yering", sur ceux qui partent
    sans laisser trace de vie ni de mort. Il fut membre du fameux trio
    Keremendeong et en composa la chanson éponyme en plus d'un hymne en hommage
    au lutteur Balla Gueye II, "Lac de guerre II". Ex-footballeur, son énergie
    et son charme émanent de son charisme scénique. Il a inventé le style
    afro-djambo et le propage à l'échelle internationale.
  </p>
</main>

<svelte:window bind:scrollY={Y} />

<style lang="scss">
  @use "colors";

  #header {
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 2;
    padding: 10px;
    font-family: Libel;
    font-size: 6em;
    margin: 20px;
    text-align: center;
    margin: 0;
    transition: all .4s;
    &.scrolled {
      font-size: 3em;
      letter-spacing: 20px;
      background-color: colors.$background_color;
    }
  }

  p.spacer {
    height: 125px;
  }

  #title {
    position: absolute;
    right: 81px;
    top: 700px;
    font-size: 9em;
    font-family: Libel;
    line-break: normal;
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
