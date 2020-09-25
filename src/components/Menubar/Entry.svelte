<script>
  // Usage: <Entry id="id">Name</Entry>

  export let id;

  import { createEventDispatcher } from "svelte";
  const dispatch = createEventDispatcher();
</script>

<style>
  span {
    min-width: 200px;
    cursor: pointer;

    display: inline-flex;
    align-items: center;
    justify-content: center;
    
    user-select: none;
  }
</style>

<span on:click={() => dispatch('click', id)}><slot /></span>
