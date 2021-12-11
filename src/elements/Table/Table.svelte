<script>
  export let customClass = "";

  export let striped = false;

  export let hover = false;

  export let scroll = false;

  $: getComputedClasses = () => {
    const classes = ["table"];

    if (striped) {
      classes.push("table-striped");
    }

    if (hover) {
      classes.push("table-hover");
    }

    if (scroll) {
      classes.push("table-scroll");
    }

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<table {...$$restProps} class={getComputedClasses()}>
  <slot />
</table>
