<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Runes effects</h3>

	<Code id="code" lines={true}
		>{`
<script>
	let size = $state(50);
	let color = $state('#ff3e00');

	let canvas;

	$effect(() => {
		const context = canvas.getContext('2d');
		context.clearRect(0, 0, canvas.width, canvas.height);

		// this will re-run whenever 'color' or 'size' change
		context.fillStyle = color;
		context.fillRect(0, 0, size, size);
	});
<\/script>

<canvas bind:this={canvas} width="100" height="100" />
`}</Code
	>

	<p>avoid overusing it!!</p>
</Slide>
