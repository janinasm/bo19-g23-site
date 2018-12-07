<template>
  <section class="blog-menu">
    <div class="blog-menu__item">Blog item 1</div>
    <div class="blog-menu__item">Blog item 2</div>
    <div class="blog-menu__item">Blog item 3</div>
    <div class="blog-menu__item">Blog item 4</div>
    <div class="blog-menu__overlay">Blog overlay</div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.blog-menu {
  grid-column: 3 / 4;
  grid-row: 2;
  background: $primary-color--dark;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(20rem, 1fr));
  grid-template-rows: repeat(2, 1fr);
  position: relative;
  &__item {
    background: $primary-color--light;
    transition: background 0.1s ease-in-out;
    &:hover,
    &:active {
      background: $primary-color--dark;
    }
    display: grid;
    align-items: center;
    align-content: center;
    justify-items: center;
    & > div {
      width: 80%;
      height: 100%;
      & > img {
        max-width: 100%;
        object-fit: scale-down;
      }
    }
  }
  &__overlay {
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: 10;
    background: gray;

    display: grid;
    align-content: center;
    justify-content: center;
  }

  @media only screen and (max-width: $bp-large) {
    grid-column: 1;
    grid-row: 3;
  }
}
</style>


