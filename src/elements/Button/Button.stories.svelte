<script>
  import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
  import Button from "./Button.svelte";
</script>

<Meta title="Elements/Button" component={Button} />

<Template let:args>
  <Button {...args} />
</Template>

<Story
  name="Default"
  args={{
    label: "Default",
  }}
/>

<Story
  name="Primary"
  args={{
    label: "Primary",
    variant: "primary",
  }}
/>

<Story
  name="Success"
  args={{
    label: "Success",
    variant: "success",
  }}
/>

<Story
  name="Error"
  args={{
    label: "Error",
    variant: "error",
  }}
/>

<Story
  name="Link"
  args={{
    label: "Link",
    variant: "link",
  }}
/>

<Story
  name="Small"
  args={{
    label: "Small",
    size: "sm",
  }}
/>

<Story
  name="Large"
  args={{
    label: "Large",
    size: "lg",
  }}
/>

<Story
  name="Loading"
  args={{
    label: "Loading",
    loading: true,
  }}
/>

<Story
  name="Disabled"
  args={{
    label: "Disabled",
    disabled: true,
    variant: "primary",
  }}
/>

<Story name="Circle Icon">
  <Button variant="primary" action circle>
    <i class="icon icon-arrow-left" />
  </Button>
</Story>
