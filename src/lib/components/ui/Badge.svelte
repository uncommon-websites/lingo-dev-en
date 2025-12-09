<script lang="ts">
  import { type Snippet } from 'svelte';

  let { children, class: className = '' }: { children: Snippet, class?: string } = $props();
</script>

<span class="inline-flex items-center rounded-full border border-gray-800 bg-gray-900/50 px-2.5 py-0.5 text-xs font-medium text-gray-300 backdrop-blur-sm {className}">
  {@render children()}
</span>
