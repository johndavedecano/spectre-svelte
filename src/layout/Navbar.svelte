<script>
  export let customClass = "";

  $: getComputedClasses = () => {
    const classes = ["navbar"];

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<header {...$$restProps} class={getComputedClasses()}>
  <slot />
</header>
