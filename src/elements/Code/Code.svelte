<script>
  export let language = "HTML";

  export let customClass = "";

  $: getComputedClasses = () => {
    const classes = ["code"];

    if (customClass) {
      classes.push(customClass);
    }

    return classes.join(" ");
  };
</script>

<pre {...$$restProps} class={getComputedClasses()} data-lang={language}>
  <code>
    <slot />
  </code>
</pre>
