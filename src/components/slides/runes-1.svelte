<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Runes</h3>
	<p>A letter or mark used as a mystical or magic symbol.</p>
	<p>Runes have a "$" prefix and look like functions:</p>
	<Code id="code" lines={false}
		>{`
<script>
    let message = $state('hello'); 
<\/script>
`}</Code
	>

	<p>
		Now you can also use svelte runes in ".svelte.js" or ".svelte.ts", it's not only limited to
		".svelte" files
	</p>
</Slide>
