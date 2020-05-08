<script>
  import NavLink from "./NavLink";
  export let segment;
  let links = [
    {
      name: "Home",
      link: "."
    },
    {
      name: "About",
      link: "about"
    },
    {
      name: "Login",
      link: "login"
    },
    {
      name: "Register",
      link: "register"
    }
  ];
</script>

<style>

</style>

<header
  class="flex justify-between items-center sm:px-18 px-6 text-gray-800 md:px-24
  border-b-2 bg-white">
  <div>
    <h1 class="text-3xl">Auction</h1>
  </div>
  <div class="">
    <div class="flex">
      {#each links as link}
        <NavLink {segment} name={link.name} link={link.link} />
      {/each}
    </div>
  </div>
</header>
