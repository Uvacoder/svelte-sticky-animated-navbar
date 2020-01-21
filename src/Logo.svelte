<script>
  import { dark } from "./store.js";
  let y;
  $: logo = $dark ? "/logo-dark.png" : "/logo.png";
</script>

<style lang="scss">
  img {
    width: 400px;
    max-width: 40vw;
    padding: 10px;
    position: fixed;
    transition: all 0.5s;
    z-index: 1;
  }
  .small {
    width: 14rem;
  }
</style>

<img src={logo} alt="Logo" class:small={y > 50} />

<svelte:window bind:scrollY={y} />
