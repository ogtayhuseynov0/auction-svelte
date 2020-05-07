<script>
  export let segment;

  $: checkActive = active => {
    return segment === active;
  };
</script>

<style>
  .nov {
    border-radius: 0;
  }
</style>

<div class="ui inverted segment nov">
  <div class="ui inverted secondary menu container menu">
    <div class="menu">
      <span class="item header" style="font-size:1.2em">Auction</span>
    </div>
    <div class="menu right">
      <a class="item" href="." class:active={checkActive(undefined)}>Home</a>
      <a class="item" href="about" class:active={checkActive('about')}>About</a>
      <div class="item">
        <div class="ui primary button" on:click>Log In</div>
        &nbsp;&nbsp;
        <div class="ui button">Sign Up</div>
      </div>
    </div>
  </div>
</div>
