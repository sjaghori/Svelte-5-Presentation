<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Runes Derived</h3>

	<Code id="code" lines={true}
		>{`
<script>
	let count = $state(0);
	let doubled = $derived(count * 2);
<\/script>

<button onclick={() => count++}>
	{doubled}
</button>

<p>{count} doubled is {doubled}</p>
`}</Code
	>

	<a href="#/3">Back to problem</a>
</Slide>
