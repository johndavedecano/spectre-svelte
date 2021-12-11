<script>
  export let wrapperClasses = "";

  export let bodyClasses = "";

  export let size = "";

  $: getWrapperClasses = () => {
    const classes = [];

    if (size) {
      classes.push(`hero-${size}`);
    }

    if (wrapperClasses) {
      classes.push(wrapperClasses);
    }

    return classes.join(" ");
  };

  $: getBodyClasses = () => {
    const classes = ["hero-body"];

    if (bodyClasses) {
      classes.push(bodyClasses);
    }

    return classes.join(" ");
  };
</script>

<div {...$$restProps} class={getWrapperClasses()}>
  <div class={getBodyClasses()}>
    <slot />
  </div>
</div>
