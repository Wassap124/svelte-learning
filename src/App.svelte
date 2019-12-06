<script>
  const name = "Alon";
  const src = "image.gif";
  import NestedParagraph from "../src/nested-paragraph/nested-paragraph.svelte";
</script>

<style>
  /* css goes here */
  .main {
    text-align: center;
    margin: 0;
  }
</style>

<div class="main">
  <h1>Hello {name.toLowerCase()}!</h1>
  <img {src} alt="You have been rick rolled by {name}" />
  <NestedParagraph />
</div>
