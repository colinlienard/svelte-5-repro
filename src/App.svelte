<script lang="ts">
  import type { Action } from "svelte/action";

  const action: Action<HTMLElement, { foo: string }> = (node, { foo }) => {
    console.log(node, foo);
  };
</script>

<div use:action={{ foo: "bar" }}></div>
