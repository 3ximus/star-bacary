<div class="about">
  <img src="bacary.png" alt="" />
  <div class="text">
    <h1>À propos de l'artiste</h1>
    <p class="bio">
      Avec sa maîtrise parfaite du rythme africain du 21e siècle, à la frontière
      du mystique, Star Bacary est résolument tourné vers le monde. Bacary né
      Sonko est originaire du département de Goudomp, près de Ziguinchor, là où
      coulent les murmures du fleuve Casamance.
      <br />
      <br />
      Très tôt conscientisé aux maux de la société africaine dont le sort incertain
      de la jeunesse, il ouvre grand les yeux sur les déroutes des politiciens à
      l'égard de sa génération. Il devient leur porte-voix, d'ouest en est de sa
      Casamance, et à travers la diaspora.
      <br />
      <br />
      Le destin tragique de ses amis exilés dans de fatales « pirogues cercueils
      » le pousse à écrire sa première chanson en 2012, à l'âge de 19 ans "Immigration
      clandestine"/"Toukou toukou yering", sur ceux qui partent sans laisser trace
      de vie ni de mort.
      <br />
      <br />
      Il fut membre du fameux trio Keremendeong et en composa la chanson éponyme
      en plus d'un hymne en hommage au lutteur Balla Gueye II, "Lac de guerre II".
      Ex-footballeur, son énergie et son charme émanent de son charisme scénique.
      Il a inventé le style afro-djambo et le propage à l'échelle internationale.
    </p>
  </div>

  <!-- https://www.facebook.com/starbakay/ -->

</div>

<style lang="scss">
  div.about {
    display: flex;
    align-items: center;
    img {
      height: 100vh;
      margin-left: 60px;
    }
    div.text {
      max-width: 40%;
      h1 {
        font-family: Libel;
      }
      p.bio {
        font-size: 1.2em;
        text-align: justify;
      }
    }
  }

  @media (max-width: 800px) {
    div.about {
      justify-content: center;
      flex-direction: column-reverse;
      img {
        height: 60vh
      }
      div.text {
        max-width: 90%;
      }
    }
  }
</style>
