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
          A tower defense game with permadeath and roguelike progression. You
          have to defeat 50 increasingly difficult waves without losing your
          core. Each wave grants you randomly rolled rewards like towers,
          upgrades, abilities and modules.
        </Project>
        <Project
          title="FRGMNTS"
          url="https://coredefense.ehmprah.com"
          image="/screenshot_core_defense.png"
        >
          A tower defense game with permadeath and roguelike progression. You
          have to defeat 50 increasingly difficult waves without losing your
          core. Each wave grants you randomly rolled rewards like towers,
          upgrades, abilities and modules.
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

// TODO add google analytics
// TODO set page title

export default {
  components: {
    Follow,
    Project
  }
};
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

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
}

.footer {
  margin: 4em 0 2em 0;
}
</style>
