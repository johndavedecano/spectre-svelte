<script>
  export let customClass = "";

  export let col = "";

  export let xs = "";

  export let sm = "";

  export let md = "";

  export let lg = "";

  export let xl = "";

  export let offset = "";

  $: getComputedClasses = () => {
    const classes = ["column"];

    if (col) {
      classes.push(`col-${col}`);
    }

    if (xs) {
      classes.push(`col-xs-${xs}`);
    }

    if (sm) {
      classes.push(`col-sm-${sm}`);
    }

    if (md) {
      classes.push(`col-md-${md}`);
    }

    if (lg) {
      classes.push(`col-lg-${lg}`);
    }

    if (xl) {
      classes.push(`col-xl-${xl}`);
    }

    if (offset) {
      classes.push(`col-${offset}-auto`);
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
