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
      classes.push('show-xs');
    }

    if (sm) {
      classes.push('show-sm');
    }

    if (md) {
      classes.push('show-md');
    }

    if (lg) {
      classes.push('show-lg');
    }

    if (xl) {
      classes.push('show-xl');
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
