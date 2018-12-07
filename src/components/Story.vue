<template>
  <section class="story">
    <h1 class="story__headline headline--xl">Bacheloroppgaven 2019</h1>
    <h2 class="story__subtitle headline--m">BO19-G23 Janina Simone Martinsen</h2>
    <p class="story__text text--s">Text 1</p>
    <p class="story__text text--s">Text 2</p>
    <div class="story__portrait">
      <img src alt>
    </div>
    <div class="story__docs text--s">
      <a href class="story__docs__item">Link 1</a>
      <a href class="story__docs__item">Link 2</a>
      <a href class="story__docs__item">Link 3</a>
      <a href class="story__docs__item">Link 4</a>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.story {
  grid-column: 1 / 3;
  grid-row: 1 / -1;
  background: $primary-color;
  color: $base-color--light;
  padding: 7rem 8vw;
  display: grid;
  grid-gap: 2rem;
  align-content: center;
  &__headline {
  }
  &__subtitle {
  }
  &__text {
  }
  &__portrait {
    width: 25rem;
    height: 25rem;
    border-radius: 50%;
    background: gray;
  }
  &__docs {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(5rem, 1fr));

    &__item {
      color: $base-color--light;
    }
  }
  @media only screen and (max-width: $bp-large) {
    grid-column: 1;
    grid-row: 1;
  }
}
</style>
