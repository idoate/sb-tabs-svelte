<button on:click={ ()=> setThisTab(tabText) } >
	{ tabName }
</button>



<script lang="ts">
  import { createEventDispatcher } from "svelte";
  const dispatcher = createEventDispatcher();
  export let tabName = "";
  export let tabText = "";
  function setThisTab(tabText) {
    dispatcher("setCurrentTabText", tabText);
  }
</script>