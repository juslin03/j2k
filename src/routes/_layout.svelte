<script>
  import { onMount } from "svelte";
  import Nav from "../components/Nav.svelte";

  import { quintIn } from "svelte/easing";
  import { fade } from "svelte/transition";

  onMount(() => {});

  let visible = true;
  let isClick = false;

  function home(e) {
    location.replace(e.explicitOriginalTarget.baseURI);
  }

  function contextDisable(e) {
    e.preventDefault();
  }
</script>

<header
  on:contextmenu={contextDisable}
  class="section section--header"
  id="logo"
>
  <p transition:fade={{ x: -200, duration: 2000 }} class="textwriter">
    Je suis Juslin Komenan!
  </p>
  <img on:click={home} class="profil" src="juslin-profil.png" alt="" />
</header>
<main on:contextmenu={contextDisable} class="section section--main">
  <slot />
</main>

<style>
  img {
    cursor: pointer;
  }
  .textwriter {
    padding: 10px;
    text-align: center;
    text-transform: uppercase;
    width: 100%;
    position: relative;
    top: -180px;
    color: white;
    background-color: black;
  }
</style>
