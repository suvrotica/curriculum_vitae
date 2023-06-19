<script>
  import MarkdownEditor from "../lib/components/MarkdownEditor.svelte";
  import Education from "../lib/components/Education.svelte";
  let phone_icon_image = "/Images/phone.svg";
</script>

<main class="container">
  <Education {phone_icon_image} />
</main>

<style>
  main {
    margin: auto;
    width: 95%;
  }
</style>
