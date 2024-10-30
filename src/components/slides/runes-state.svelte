<script lang="ts">
	import Code from '../deck/code.svelte';
	import Slide from '../deck/slide.svelte';
</script>

<Slide animate>
	<h3>Runes State - Classes</h3>

	<Code id="code" lines={true}
		>{`
class Todo {
	done = $state(false);
	text = $state();

	constructor(text) {
		this.text = text;
	}

	reset() {
		this.text = '';
		this.done = false;
	}
}
`}</Code
	>
</Slide>
