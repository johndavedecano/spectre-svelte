<script>
  export let customClass = "";

  export let gapLess = false;

  export let oneLine = false;

  $: getComputedClasses = () => {
    const classes = ["columns"];

    if (gapLess) {
      classes.push("col-gapless");
    }

    if (oneLine) {
      clases.push("col-oneline");
    }

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<div {...$$restProps} class={getComputedClasses()}>
  <slot />
</div>
