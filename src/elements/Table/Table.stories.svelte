<script>
  import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
  import Table from "./Table.svelte";
</script>

<Meta title="Elements/Table" component={Table} />

<Template let:args>
  <Table {...args} />
</Template>

<Story name="Default">
  <Table>
    <thead>
      <tr>
        <th>name</th>
        <th>genre</th>
        <th>release date</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
    </tbody>
  </Table>
</Story>


<Story name="Striped">
  <Table striped>
    <thead>
      <tr>
        <th>name</th>
        <th>genre</th>
        <th>release date</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
    </tbody>
  </Table>
</Story>

<Story name="Hover">
  <Table hover>
    <thead>
      <tr>
        <th>name</th>
        <th>genre</th>
        <th>release date</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
    </tbody>
  </Table>
</Story>

<Story name="Scrollable">
  <Table style="max-width:200px;" scroll>
    <thead>
      <tr>
        <th>name</th>
        <th>genre</th>
        <th>release date</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
      <tr>
        <td>The Shawshank Redemption</td>
        <td>Crime, Drama</td>
        <td>14 October 1994</td>
      </tr>
    </tbody>
  </Table>
</Story>
