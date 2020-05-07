<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
</script>

<style>

</style>

<Nav {segment} />

<main>
  <div class="container ui">
    <slot />
  </div>
</main>
