<script lang="ts">
  import { onMount } from "svelte";

  import "@picocss/pico";
  let fontLoaded = false;

  let fontLink;

  onMount(() => {
    fontLink = document.createElement("link");
    fontLink.href =
      "https://fonts.googleapis.com/css2?family=Gaegu:wght@300;400;700&family=Poppins:ital,wght@0,100;1,100&family=Montserrat:wght@300&family=Amatic+SC:wght@400;700&display=swap";
    fontLink.rel = "stylesheet";
    fontLoaded = true;
    document.head.appendChild(fontLink);
  });

  import Navigation from "$lib/components/Navigation.svelte";
  import SectionHeader from "$lib/components/SectionHeader.svelte";
</script>

<main class="container">
  <article>
    <header>
      <Navigation />
    </header>
    <SectionHeader>
      <p slot="leftContent">CURRICULUM VITAE</p>
      <p slot="rightContent">EDUCATION</p>
    </SectionHeader>
    <slot />
    <SectionHeader>
      <p slot="leftContent">CURRICULUM VITAE</p>
      <p slot="rightContent">WORK</p>
    </SectionHeader>
    <footer>Footer</footer>
  </article>hello J
</main>

<style>
  header {
    transform: rotate(2deg);
  }
  footer {
    transform: rotate(2deg);
  }

  :global(body) {
    font-family: "Gaegu", cursive;
    font-weight: 300;
  }
  :global(h1, h2, h3, h4, h5, h6) {
    font-family: "Amatic SC", cursive;
  }
</style>
