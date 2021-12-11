<script>
  export let customClass = "";

  $: getComputedClasses = () => {
    const classes = ["container"];

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<div {...$$restProps} class={getComputedClasses()}>
  <slot />
</div>
