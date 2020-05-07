<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
</script>

<style>

</style>

<Nav {segment} />

<main>
  <div class="px-6 sm:px-18 md:px-24 mt-2">
    <slot />
  </div>
</main>
