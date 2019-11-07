<template>
  <div class="container">
    <div>
      <div class="about">
        <img class="about__img" src="~assets/ehmprah.png" />
        <h1 class="about__heading">Hi, I'm ehmprah!</h1>
        <div class="about__description">
          I am a developer of games and things and I write a lot in my free
          time. I work at
          <a href="https://twitter.com/sevenval" target="_blank">@sevenval</a>
          and always on multiple side projects, which you will find below.
        </div>
        <!-- TODO: add follow icons -->
      </div>
      <div class="projects">
        <div class="project">
          <a
            href="https://coredefense.ehmprah.com"
            target="_blank"
            class="project__screenshot"
          >
            <img src="~assets/screenshot_core_defense.png" />
          </a>
          <div class="project__info">
            <h2 class="project__heading">Core Defense</h2>
            <div class="project__description">
              A tower defense game with permadeath and roguelike progression.
              You have to defeat 50 increasingly difficult waves without losing
              your core. Each wave grants you randomly rolled rewards like
              towers, upgrades, abilities and modules.
            </div>
            <a class="project__button" href="https://coredefense.ehmprah.com"
              >Check it out</a
            >
          </div>
        </div>
      </div>

      <div class="footer">
        <a href="/imprint">Imprint</a>
        <!-- TODO style imprint! -->
      </div>
    </div>
  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue';
// TODO create project component with named slots

export default {
  // components: {
  //   Logo
  // }
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
  background: #222;
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

.project {
  display: flex;
  align-items: center;

  &__heading {
    color: #ff0083;
    line-height: 1.5em;
    font-size: 1.5em;
  }

  &__info {
    text-align: left;
  }

  &__description {
    text-align: justify;
    margin: 0 0 1em 0;
  }

  &__screenshot {
    border: none;
    display: block;
    margin-right: 1.5em;
    &:hover {
      border: none;
    }
  }

  &__button {
    background: #ff0083;
    border-radius: 4px;
    display: inline-block;
    border: none;
    padding: 0.5em 1em;
    color: white;
    &:hover {
      border: none;
      color: white;
    }
  }
}

.footer {
  margin: 2em 0;
}
</style>
