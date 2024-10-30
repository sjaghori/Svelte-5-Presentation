<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Migration</h3>
	<p>From Svelte 4 to Svelte 5, there is a migration script</p>

	<Code id="code" lines={true}
		>{`
npx sv migrate
`}</Code
	>
</Slide>
