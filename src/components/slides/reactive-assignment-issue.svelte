<script lang="ts">
	import Notes from "../deck/notes.svelte";
	import Code from "../deck/code.svelte";
	import Slide from "../deck/slide.svelte";
</script>

<Slide animate>
	<Code id="code" lines="0|4|2-3">
		{`<script>
			let count = 1;
			$: double = count * 2;
			console.log(double);
		</script>
		
		<button on:click={() => {
			count++;
			console.log(count, double);
		}}>count: {count}, double: {double}</button>`}
	</Code>

	<Notes>
	</Notes>
</Slide>
