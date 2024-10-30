<script lang="ts">
	import Code from "../deck/code.svelte";
	import Slide from "../deck/slide.svelte";
</script>

<Slide animate>
    <h4 class="mb-4">Compatibility</h4>

    <p>It is possible to use Svelte 3 components in Svelte 5 (but probably not in Svelte 6)</p>

    <Code id="code" lines={false}>
		{`
	"devDependencies": {
		"@sveltejs/vite-plugin-svelte": "^3.0.0",
		"svelte": "^4",
		// …
	}
}`}
	</Code>

    <Code id="code" lines={false}>
		{`
	"devDependencies": {
		"@sveltejs/vite-plugin-svelte": "^4.0.0",
		"svelte": "^5",
		// …
	}
}`}
	</Code>
</Slide>
