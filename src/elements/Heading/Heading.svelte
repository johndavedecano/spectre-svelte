<script>
  export let label = "";

  export let variant = "h1";

  export let customClass;

  $: getComputedClasses = () => {
    const classes = [];
    const variants = ["h1", "h2", "h3", "h4", "h5", "h6"];

    if (variants.includes(variant)) {
      classes.push(variant);
    }

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<div {...$$restProps} class={getComputedClasses()}>
  <slot>{label}</slot>
</div>
