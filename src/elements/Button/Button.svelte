<script>
  export let label = "";

  export let variant = "default";

  export let size = "md";

  export let type = "button";

  export let loading = false;

  export let disabled = false;

  export let circle = false;

  export let action = false;

  export let customClass = "";

  const variants = {
    primary: "btn-primary",
    link: "btn-link",
    success: "btn-success",
    error: "btn-error",
  };

  const sizes = {
    sm: "btn-sm",
    md: undefined,
    lg: "btn-lg",
  };

  $: getComputedClasses = () => {
    const classes = ["btn"];

    if (variants[variant]) {
      classes.push(variants[variant]);
    }

    if (sizes[size]) {
      classes.push(sizes[size]);
    }

    if (loading) {
      classes.push("loading");
    }

    if (disabled) {
      classes.push("disabled");
    }

    if (action) {
      classes.push("btn-action");
    }

    if (circle) {
      classes.push("s-circle");
    }

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<button {...$$restProps} {type} {disabled} class={getComputedClasses()}>
  <slot>{label}</slot>
</button>
