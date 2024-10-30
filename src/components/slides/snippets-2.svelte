<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Snippets create reusable chunks of markup</h3>

	<Code id="code" lines={true}
		>{`
<script>
	let { message = 'it's great to see you!' } = $props();
<\/script>

{#snippet hello(name)}
	<p>hello {name}! {message}!</p>
{/snippet}

{@render hello('alice')}
{@render hello('bob')}
`}</Code
	>
</Slide>
