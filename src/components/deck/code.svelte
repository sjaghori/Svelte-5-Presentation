<script lang="ts">
	import type { Snippet } from 'svelte';

	type CodeProps = {
		id: string | null;
		lines: string | boolean | null;
		noescape?: boolean;
		children: Snippet<[]>;
	}

	let { id = null, lines = null, noescape = false, children }: CodeProps = $props();
</script>

<pre data-id={id || null}>
  <code data-trim data-line-numbers={lines || null} data-noescape={noescape || null}>
  {@render children()}
  </code>
</pre>
