<style>
  header {
    height: 50vh;
    background-image: url(/background.jpg);
    background-size: cover;
    background-position: 0% 25%;
    clip-path: polygon(0 0, 100% 0, 100% 90%, 0 100%);
  }
</style>

<header>
  <slot name="logo" />
  <slot />
</header>