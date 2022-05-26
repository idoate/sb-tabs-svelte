<script>
    import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
    import Tab from "./Tab.svelte";

</script>

<Meta
        title="Tab"
        component={Tab}
/>

<Template let:args>
    <Tab {...args} />
</Template>

<Story
        name="Primary"
        args={{
    tabName: 'tab 1',
    tabText: 'Texto do primeiro tab',
};
  }}
/>

