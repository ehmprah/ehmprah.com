<template>
  <div class="project">
    <a :href="url" target="_blank" class="project__screenshot">
      <img :src="image" />
    </a>
    <div class="project__info">
      <h2 class="project__heading">{{ title }}</h2>
      <div class="project__description">
        <slot></slot>
      </div>
      <a class="project__button" :href="url">Check it out</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Project',
  props: {
    url: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    }
  }
};
</script>

<style lang="scss">
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
    display: block;
    text-align: center;
    border: none;
    padding: 0.5em 1em;
    color: white;
    &:hover {
      border: none;
      color: white;
    }
  }
}
</style>
