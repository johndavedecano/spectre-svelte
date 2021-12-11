<script>
  export let customClass = "";

  $: getComputedClasses = () => {
    const classes = ["navbar-section"];

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<section {...$$restProps} class={getComputedClasses()}>
  <slot />
</section>
