<script>
  export let block = false;

  $: getComputedClasses = () => {
    const classes = ["btn-group"];

    if (block) {
      classes.push("btn-group-block");
    }

    return classes.join(" ");
  };
</script>

<div {...$$restProps} class={getComputedClasses()}>
  <slot />
</div>
