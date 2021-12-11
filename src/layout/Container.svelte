<script>
  export let customClass = "";

  export let maxWidth = "";

  $: getComputedClasses = () => {
    const classes = ["container"];

    if (maxWidth) {
      classes.push(`grid-${maxWidth}`);
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
