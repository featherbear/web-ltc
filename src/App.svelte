<script>
  import Router from "svelte-spa-router";
  import Menubar from "./components/Menubar/Menubar.svelte";

  function handleAction(action) {
    alert("Action " + action);
  }
</script>

<style lang="scss">
  div.mainContainer {
    min-height: 100%;
    /* min-height: 100%; */
    display: flex;
    flex-direction: column;

    main {
      flex: 1;
      text-align: center;
      //   padding: 1em;
      max-width: 240px;
      margin: 0 auto;
    }
    footer {
      border-top: 1px solid grey;
    }
  }
</style>

<div class="mainContainer">
  <main>
  </main>
  <footer>
    <Menubar on:click={({ detail: action }) => handleAction(action)} />
  </footer>
</div>
