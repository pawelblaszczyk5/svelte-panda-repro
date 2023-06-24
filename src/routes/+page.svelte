<script context="module">
  let styleModule = css({ color: "yellow.400" });
</script>

<script>
  import { css } from "styled-system/css";

  let style = css({ color: "green.400" });
</script>

<h1 class={style}>using class binding css</h1>
<div
  class={css({
    padding: "40px",
    color: "red.700",
    fontSize: "3xl",
  })}
>
  It works in Svelte, using inline styles
</div>
<p class={styleModule}>
  It doesn't work in Svelte using script context binding
</p>
