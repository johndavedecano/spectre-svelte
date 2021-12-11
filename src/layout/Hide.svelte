<script>
  export let customClass = "";

  export let xs = false;

  export let sm = false;

  export let md = false;

  export let lg = false;

  export let xl = false;

  $: getComputedClasses = () => {
    const classes = [];

    if (xs) {
      classes.push('hide-xs');
    }

    if (sm) {
      classes.push('hide-sm');
    }

    if (md) {
      classes.push('hide-md');
    }

    if (lg) {
      classes.push('hide-lg');
    }

    if (xl) {
      classes.push('hide-xl');
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
