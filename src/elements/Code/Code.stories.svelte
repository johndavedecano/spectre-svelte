<script>
  import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
  import Code from "./Code.svelte";
</script>

<Meta title="Elements/Code" component={Code} />

<Template let:args>
  <Code {...args} />
</Template>

<Story name="Default">
  <Code language="HTML">
    <span class="com">&lt;!-- code snippets --&gt;</span>
    &lt;<span class="tag">button</span> <span class="atn">class</span>=<span class="atv">&quot;btn&quot;</span>&gt;
      Submit
    &lt;<span class="tag">/button</span>&gt;
  </Code>
</Story>
