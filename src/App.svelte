<div>
	<h1>Tabs in svelte</h1>
	<Home tabs1='{tabs}' />
</div>

<script lang="ts">
import Home from "./components/Home/Home.svelte";
const tabs = [
	{
		name:'tab 1',
		text:'Texto do primeiro tab'
	},
	{
		name:'tab 2',
		text:'Texto do segundo tab'
	},
	{
		name:'tab 3',
		text:'Texto do terceiro tab'
	},
	{
		name:'tab 4',
		text:'Texto do quarto tab'
	}
]
</script>

