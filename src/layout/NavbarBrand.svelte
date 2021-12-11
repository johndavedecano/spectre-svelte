<script>
  export let customClass = "";

  export let href = "/";

  $: getComputedClasses = () => {
    const classes = ["navbar-brand"];

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<a {...$$restProps} {href} class={getComputedClasses()}>
  <slot />
</a>
