<template>
  <div class="container">
    <div class="imprint">
      <h1 class="imprint__heading">Imprint</h1>
      <div>
        <p>
          Mario Kaiser<br />
          Graudenzer Str. 17<br />10243 Berlin
        </p>
        <p>Email: <a href="mailto:ehmprah@gmail.com">ehmprah@gmail.com</a></p>
      </div>
      <a href="/">Back</a>
    </div>
  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue';

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
}

.imprint {
  width: 80vw;
  max-width: 480px;
  margin: 3em auto;
  &__heading {
    font-size: 2em;
    line-height: 1.5em;
    color: #ff0083;
    margin-bottom: 0.5em;
  }
}
</style>
