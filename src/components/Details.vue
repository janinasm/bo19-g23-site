<template>
  <section class="details">
    <h2 class="details__headline headline--m"></h2>
    <p class="details__text text--s"></p>
  </section>
</template>

<script>

export default {
 
}
</script>

<style scoped lang="scss">

.details {
    grid-column: 3 / -1;
    grid-row: 1;
    background: #ffffee;
    display: grid;
    padding: 7rem 8vw;
    grid-gap: 2rem;
    align-content: start;
    &__headline {}

    @media only screen and (max-width: $bp-large) {
        grid-column: 1;
        grid-row: 2;
    }
}
</style>
