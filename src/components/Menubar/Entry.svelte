<script>
  // Usage: <Entry path="path">Name</Entry>

  export let path;

  import { createEventDispatcher } from "svelte";
  const dispatch = createEventDispatcher();
</script>

<style lang="scss">
  span {
    min-width: 200px;
    cursor: pointer;

    display: inline-flex;
    align-items: center;
    justify-content: center;
    
    user-select: none;
  }
</style>

<span on:click={() => dispatch('click', path)}><slot /></span>
