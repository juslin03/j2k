<script>
  import Nav from "../components/Nav.svelte";

  import { quintOut } from "svelte/easing";
  import { fade, draw, fly } from "svelte/transition";

  let visible = true;
  let isClick = false;

  function home(e) {
    location.replace(e.explicitOriginalTarget.baseURI);
  }

  function contextDisable(e) {
    e.preventDefault();
  }
</script>

<style>
  img {
    cursor: pointer;
  }
</style>

<header
  on:contextmenu={contextDisable}
  class="section section--header"
  id="logo">
  <img on:click={home} class="profil" src="juslin.jpeg" alt="" />
</header>
<main
  on:contextmenu={contextDisable}
  class="section section--main">
  <slot />
</main>
