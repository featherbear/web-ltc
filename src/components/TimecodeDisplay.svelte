<script>
  export let hour = 0;
  export let minute = 0;
  export let second = 0;
  export let frame = 0;

  const pad = (i) => i.toString().padStart(2, "0");
</script>

<style>
  span {
    /* font-family: 'monospace'; */
    font-size: 4em;
  }
</style>
<span>
  {pad(hour)}:{pad(minute)}:{pad(second)}:{pad(frame)}
</span>
