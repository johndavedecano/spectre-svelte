<script>
  import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
  import Heading from "./Heading.svelte";
</script>

<Meta title="Elements/Typography" component={Heading} />

<Template let:args>
  <Heading {...args} />
</Template>

<Story name="Headings">
  <div>
    <Heading variant="h1">Heading 1 - 40px</Heading>
    <Heading variant="h2">Heading 2 - 32px</Heading>
    <Heading variant="h3">Heading 3 - 28px</Heading>
    <Heading variant="h4">Heading 4 - 24px</Heading>
    <Heading variant="h5">Heading 5 - 20px</Heading>
    <Heading variant="h6">Heading 6 - 16px</Heading>
  </div>
</Story>

<Story name="Paragraphs">
  <p>
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent risus leo,
    dictum in vehicula sit amet, feugiat tempus tellus. Duis quis sodales risus.
    Etiam euismod ornare consequat.
  </p>
</Story>

<Story name="Lists">
  <div>
    <!-- unordered list -->
    <ul>
      <li>list item 1</li>
      <li>
        list item 2
        <ul>
          <li>list item 2.1</li>
          <li>list item 2.2</li>
          <li>list item 2.3</li>
        </ul>
      </li>
      <li>list item 3</li>
    </ul>

    <!-- description list -->
    <dl>
      <dt>description list term</dt>
      <dd>description list description</dd>
    </dl>
  </div>
</Story>

<Story name="Blockquote">
  <blockquote>
    <p>
      The advance of technology is based on making it fit in so that you don't
      really even notice it, so it's part of everyday life.
    </p>
    <cite>- Bill Gates</cite>
  </blockquote>
</Story>

<Story name="Text Elements">
  <div class="docs-demo columns">
    <div class="column col-6 col-xs-12">
      <abbr title="Internationalization">I18N</abbr><code class="ml-2"
        >abbr</code
      >
    </div>
    <div class="column col-6 col-xs-12">
      <strong>Bold</strong><code class="ml-2">strong</code><code class="ml-2"
        >b</code
      >
    </div>
    <div class="column col-6 col-xs-12">
      <cite>Citation</cite><code class="ml-2">cite</code>
    </div>
    <div class="column col-6 col-xs-12">
      <code>Hello World!</code><code class="ml-2">code</code>
    </div>
    <div class="column col-6 col-xs-12">
      <del>Deleted</del><code class="ml-2">del</code>
    </div>
    <div class="column col-6 col-xs-12">
      <em>Emphasis</em><code class="ml-2">em</code>
    </div>
    <div class="column col-6 col-xs-12">
      <i>Italic</i><code class="ml-2">i</code>
    </div>
    <div class="column col-6 col-xs-12">
      <ins>Inserted</ins><code class="ml-2">ins</code>
    </div>
    <div class="column col-6 col-xs-12">
      <kbd>Ctrl + S</kbd><code class="ml-2">kbd</code>
    </div>
    <div class="column col-6 col-xs-12">
      <mark>Highlighted</mark><code class="ml-2">mark</code>
    </div>
    <div class="column col-6 col-xs-12">
      <ruby
        >漢
        <rt>kan</rt>字
        <rt>ji</rt>
      </ruby><code class="ml-2">ruby</code>
    </div>
    <div class="column col-6 col-xs-12">
      <s>Strikethrough</s><code class="ml-2">s</code>
    </div>
    <div class="column col-6 col-xs-12">
      <samp>Sample</samp><code class="ml-2">samp</code>
    </div>
    <div class="column col-6 col-xs-12">
      Text <sub>Subscripted</sub><code class="ml-2">sub</code>
    </div>
    <div class="column col-6 col-xs-12">
      Text <sup>Superscripted</sup><code class="ml-2">sup</code>
    </div>
    <div class="column col-6 col-xs-12">
      <time>20:00</time><code class="ml-2">time</code>
    </div>
    <div class="column col-6 col-xs-12">
      <u>Underline</u><code class="ml-2">u</code>
    </div>
    <div class="column col-6 col-xs-12">
      <var>x</var> =
      <var>y</var> + 2<code class="ml-2">var</code>
    </div>
  </div>
</Story>
