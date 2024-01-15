<script lang="ts">
  import type { Snippet } from 'svelte'

  const { children } = $props<{ children: Snippet }>()
</script>

<button>
  {@render children()}
</button>

<style>
  button {
    padding: 1rem;
    border: 1px solid red;
    background: transparent;
  }
</style>
