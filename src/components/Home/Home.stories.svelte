<script>
	import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
	import Home from "./Home.svelte";

</script>

<Meta
		title="Home"
		component={Home}
/>

<Template let:args>
	<Home {...args} />
</Template>

<Story
		name="Primary"
		args={{
    tab: [
        {
            name: 'Tab 1',
            text: 'Texto do Tab 1'
        },
        {
            name: 'Tab 2',
            text: 'Texto do Tab 2'
        },
        {
            name: 'Tab 3',
            text: 'Texto do Tab 3'
        },
        {
            name: 'Tab 4',
            text: 'Texto do Tab 4'
        }
    ]
  }}
/>

