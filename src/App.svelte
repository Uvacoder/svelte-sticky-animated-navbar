<script>
  import Header from "./Header.svelte";
  import Navbar from "./Navbar.svelte";
  import Logo from "./Logo.svelte";
  import Toggle from "./Toggle.svelte";
  export let name;
</script>

<style lang="scss" global>
  @import "./global.scss";
</style>

<Logo />
<Navbar />
<Header />

<main>
  <div class="center">
    <h2>Hello {name}</h2>
  </div>
  <div class="center">
    <Toggle />
  </div>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore, aspernatur
    praesentium non, aperiam dicta distinctio aliquid minus temporibus ullam
    provident vel, quam cumque sit earum laudantium quibusdam accusantium. Sunt,
    eius!
  </p>

  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore, aspernatur
    praesentium non, aperiam dicta distinctio aliquid minus temporibus ullam
    provident vel, quam cumque sit earum laudantium quibusdam accusantium. Sunt,
    eius!
  </p>

  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore, aspernatur
    praesentium non, aperiam dicta distinctio aliquid minus temporibus ullam
    provident vel, quam cumque sit earum laudantium quibusdam accusantium. Sunt,
    eius!
  </p>

  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore, aspernatur
    praesentium non, aperiam dicta distinctio aliquid minus temporibus ullam
    provident vel, quam cumque sit earum laudantium quibusdam accusantium. Sunt,
    eius!
  </p>

  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore, aspernatur
    praesentium non, aperiam dicta distinctio aliquid minus temporibus ullam
    provident vel, quam cumque sit earum laudantium quibusdam accusantium. Sunt,
    eius!
  </p>

  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore, aspernatur
    praesentium non, aperiam dicta distinctio aliquid minus temporibus ullam
    provident vel, quam cumque sit earum laudantium quibusdam accusantium. Sunt,
    eius!
  </p>
</main>
