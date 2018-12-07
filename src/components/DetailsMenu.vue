<template>
  <section class="details-menu">
    <div class="details-menu__item">Prosjekt</div>
    <div class="details-menu__item">Skape interesse og møte behov</div>
    <div class="details-menu__item">Moderne webteknologi</div>
    <div class="details-menu__item">Brukeropplevelse for unge og eldre</div>
  </section>
</template>

<script>
export default {
  
};
</script>

<style lang="scss" scoped>
.details-menu {
  grid-column: 4 / -1;
  grid-row: 2;
  background: $primary-color--dark;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(20rem, 1fr));
  grid-template-rows: repeat(2, 1fr);
  &__item {
    background: $primary-color--light;
    transition: background 0.1s ease-in-out;
    &:hover,
    &:active {
      background: $primary-color--dark;
    }
  }

  @media only screen and (max-width: $bp-large) {
    grid-column: 1;
    grid-row: 4;
  }
}
</style>
