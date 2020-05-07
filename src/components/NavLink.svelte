<script>
  export let name;
  export let link;
  export let segment;

  $: checkActive = active => {
    if (active === ".") active = undefined;
    return segment === active;
  };
  let changeDirect = direct => {
    window.location.replace(direct);
  };
</script>

<style>

</style>

<a
  href={link}
  class:active={checkActive(link)}
  class="block hover:text-gray-800 mr-1 hover:bg-gray-300 px-4 py-1 rounded-sm
  hidden sm:block">
  {name}
</a>
