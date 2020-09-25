<script>
  import Entry from "./Entry.svelte";
</script>

<style lang="scss">
  div.menubar {
    display: flex;
    flex-direction: row;
    min-height: 40px;
  }
</style>

<div class="menubar">
  <Entry id="home" on:click>Home</Entry>
  <Entry id="about" on:click>About</Entry>
</div>
