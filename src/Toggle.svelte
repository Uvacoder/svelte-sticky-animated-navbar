<script>
  let checked;
  $: if (checked === true) {
      trans();
      document.documentElement.setAttribute("data-theme", "dark");
  } else {
      trans();
      document.documentElement.setAttribute("data-theme", "light");
  }
  const trans = () => {
      document.documentElement.classList.add("transition");
      window.setTimeout(()=> document.documentElement.classList.remove("transition"), 1000);
  }
</script>

<style lang="scss">
  input[type="checkbox"] {
    height: 0;
    width: 0;
    visibility: hidden;
  }

  label {
    cursor: pointer;
    text-indent: -9999px;
    width: 5.2rem;
    height: 2.7rem;
    background: grey;
    float: right;
    border-radius: 100px;
    position: relative;
  }

  label:after {
    content: "";
    position: absolute;
    top: 3px;
    left: 3px;
    width: 20px;
    height: 20px;
    background: var(--color-heading);
    border-radius: 90px;
    transition: 0.3s;
  }

  input:checked + label {
    background: var(--color-bg-panel);
  }

  input:checked + label:after {
    left: calc(100% - 5px);
    transform: translateX(-100%);
  }

  label:active:after {
    width: 45px;
  }
</style>

<input type="checkbox" id="switch" bind:checked />
<label for="switch">Toggle</label>
