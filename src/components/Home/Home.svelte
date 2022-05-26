<div>
	{#each tabs1 as tabItem, index (tabItem)}
	<Tab tabName= "{tabItem.name}" tabText= "{tabItem.text}"  index={index} on:setCurrentTabText={e=>
		setCurrentTabText(e.detail)}
		/>
		{/each}
		<p>{currentTabText !== undefined  ? currentTabText : 'No tab selected yet' }</p>
</div>

<script lang="ts">
  import Tab from "../Tab/Tab.svelte";
  let currentTabText;
  export let tabs1;

  function setCurrentTabText(option) {
    currentTabText = option;
  }
</script>
