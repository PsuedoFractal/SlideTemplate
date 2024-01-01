<script lang="ts">
	import Revealer from 'reveal.js';
	import Markdown from 'reveal.js/plugin/markdown/markdown';
	import Highlight from 'reveal.js/plugin/highlight/highlight';
	import Math from 'reveal.js/plugin/math/math';
	import Notes from 'reveal.js/plugin/notes/notes';

	import 'reveal.js/dist/reveal.css';
	import 'reveal.js/dist/theme/dracula.css';
	import 'reveal.js/plugin/highlight/monokai.css';

	import Presentation from './presentation.svelte';

	import { onMount } from 'svelte';
	onMount(() => {
		const deck = new Revealer({
			plugins: [Markdown, Highlight, Math, Notes],
			controls: true,
			progress: true,
			center: true,
			transition: 'slide',
			height: 720,
			margin: 0.1,
			autoAnimate: true,
			autoAnimateDuration: 0.75
		});

		deck.initialize();
	});
</script>

<div class="reveal">
	<div class="slides">
		<Presentation />
	</div>
</div>
