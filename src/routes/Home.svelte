<script>
  import Timecode from "../components/TimecodeDisplay.svelte";

  let hour = 1;
</script>

<Timecode {hour} />

<button on:click={() => hour++}>Button</button>
