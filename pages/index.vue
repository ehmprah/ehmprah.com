<template>
  <div class="container">
    <div>
      <div class="about">
        <img class="about__img" src="/ehmprah.png" />
        <h1 class="about__heading">Hi, I'm ehmprah!</h1>
        <div class="about__description">
          I am a developer of games and things and I write a lot in my free
          time. I work at
          <a href="https://twitter.com/sevenval" target="_blank">@sevenval</a>
          and always on multiple side projects, which you will find below.
        </div>
        <Follow />
      </div>

      <div class="projects">
        <Project
          title="Core Defense"
          url="https://coredefense.ehmprah.com"
          image="/screenshot_core_defense.png"
        >
          A roguelite tower defense game with a dash of deckbuilding.
        </Project>
        <Project
          title="Climate Revolution"
          url="https://ehmprah.itch.io/climate-revolution"
          image="/screenshot_climate_revolution.png"
        >
          A card game about building political pressure to solve the climate
          crisis.
        </Project>
        <Project
          title="FRGMNTS"
          url="https://frgmnts.blog"
          image="/screenshot_frgmnts.png"
        >
          My personal blog where I write down bite-size fiction and thoughts.
        </Project>
        <Project
          title="FRGMNTS Fiction Podcast"
          url="https://frgmnts.blog/podcast.html"
          image="/podcast_thumb_wide.png"
        >
          I not only write fiction, I also read it to you. If you're into that
          kind of thing.
        </Project>
        <Project
          title="handbuch-programmieren.de"
          url="https://handbuch-programmieren.de"
          image="/screenshot_handbuch_programmieren.png"
        >
          I'm writing a free online guidebook (in German) about programming: how
          to learn it and how to get better at it.
        </Project>
        <Project
          title="programming-guidebook.com"
          url="https://programming-guidebook.com"
          image="/screenshot_programming_guidebook.png"
        >
          I'm also (slowly) translating said guidebook to English. Why? Because
          I can!
        </Project>
        <Project
          title="Geometric Tattoo Generator"
          url="https://geometric-tattoo-generator.com"
          image="/screenshot_geometric_tattoo_generator.png"
        >
          I love (geometric) tattoos, so I created a generator for those. I
          <a href="https://geometric-tattoo-generator.com/about">wear one</a>
          spat out by that thing.
        </Project>
        <Project
          title="Textures"
          url="https://www.shutterstock.com/g/ehmprah?rid=255138645&utm_medium=email&utm_source=ctrbreferral-link"
          image="/screenshot_texture.jpg"
        >
          I love, photograph, collect (and sell) textures and beautiful surfaces
          I find in nature and urban environments.
        </Project>
        <Project
          title="Coregrounds"
          url="https://github.com/ehmprah/coregrounds"
          image="/screenshot_coregrounds.png"
        >
          A multiplayer tower defense game released on
          <a href="https://store.steampowered.com/app/649770/Coregrounds/"
            >Steam</a
          >
          in April 2018. Has been shut down by the end of 2018 for many reasons
          I've outlined in a lengthy
          <a href="https://frgmnts.blog/f/how-not-to-make-a-game.html"
            >blog post</a
          >. The code is open source since then.
        </Project>
      </div>

      <div class="footer">
        <a href="/imprint">Imprint</a>
      </div>
    </div>
  </div>
</template>

<script>
import Project from '~/components/Project.vue';
import Follow from '~/components/Follow.vue';

export default {
  components: {
    Follow,
    Project
  },
  head() {
    return {
      title: 'ehmprah'
    };
  }
};
</script>

<style lang="scss">
.about {
  width: 80vw;
  max-width: 480px;
  margin: 3em auto;

  &__img {
    max-width: 200px;
  }

  &__description {
    text-align: left;
    margin: 1em 0;
  }

  &__heading {
    color: #ff0083;
    line-height: 1.5em;
    font-size: 2em;
    font-weight: bold;
  }
}

.projects {
  width: 80vw;
  max-width: 720px;
  .project:nth-child(even) {
    flex-direction: row-reverse;
  }
}

.footer {
  margin: 4em 0 2em 0;
}
</style>
