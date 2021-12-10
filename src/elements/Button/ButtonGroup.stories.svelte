<script>
  import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
  import Button from "./Button.svelte";
  import ButtonGroup from "./ButtonGroup.svelte";
</script>

<Meta title="Elements/ButtonGroup" component={ButtonGroup} />

<Template let:args>
  <ButtonGroup {...args} on:click={args.onClick} />
</Template>

<Story name="Default">
  <ButtonGroup>
    <Button variant="primary">Button 1</Button>
    <Button variant="primary">Button 2</Button>
    <Button variant="primary">Button 3</Button>
    <Button variant="primary">Button 4</Button>
  </ButtonGroup>
</Story>

<Story name="Block">
  <ButtonGroup block>
    <Button variant="primary">Button 1</Button>
    <Button variant="primary">Button 2</Button>
    <Button variant="primary">Button 3</Button>
    <Button variant="primary">Button 4</Button>
  </ButtonGroup>
</Story>
