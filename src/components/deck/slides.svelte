<script lang="ts">
	import Reveal from 'reveal.js';
	import Markdown from 'reveal.js/plugin/markdown/markdown';
	import Highlight from 'reveal.js/plugin/highlight/highlight';
	import Notes from 'reveal.js/plugin/notes/notes';
	import { onMount } from 'svelte';

	import 'reveal.js/dist/reveal.css';
	import 'reveal.js/dist/theme/black.css';
	import 'reveal.js/plugin/highlight/monokai.css';
	import Presentation from './presentation.svelte';

	onMount(() => {
		const deck = new Reveal({
			plugins: [Markdown, Highlight, Notes],
			autoAnimateEasing: 'ease',
			autoAnimateDuration: 0.2,
			hash: true,
			controls: true,
			progress: true,
		});

		deck.initialize();
	});
</script>

<div class="reveal">
	<div class="slides">
		<Presentation />
	</div>
</div>
