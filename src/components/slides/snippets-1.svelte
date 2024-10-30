<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Snippets replace "slots"</h3>

	<Code id="code" lines={true}
		>{`
<script>
    let { children } = $props();
<\/script>

{@render children?.()}
`}</Code
	>
</Slide>
