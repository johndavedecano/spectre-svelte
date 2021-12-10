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

<div {...$$props} class={getComputedClasses()}>
  <slot />
</div>
