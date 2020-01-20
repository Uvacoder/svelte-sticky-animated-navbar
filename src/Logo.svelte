<script>
  let y;
</script>

<style>
  img {
    width: 400px;
    max-width: 40vw;
    padding: 10px;
    position: fixed;
    transition: 0.5s;
    z-index: 1;
  }
  .small {
    width: 14rem;
  }
</style>

<img src="/logo.png" alt="logo" class:small={y > 50} />

<svelte:window bind:scrollY={y} />
