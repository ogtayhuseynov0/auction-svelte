<script>
  import AuctionCard from "../components/AuctionCard";
  import { fade } from "svelte/transition";

  let list = [1, 2, 3];
</script>

<svelte:head>
  <title>Auction</title>
</svelte:head>

<div class="flex items-center flex-wrap">
  {#each list as item}
    <AuctionCard />
  {/each}
</div>
