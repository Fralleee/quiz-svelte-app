<script context="module" lang="ts">
	import Button from '$lib/Button.svelte';

	export const prerender = true;
</script>

<svelte:head>
	<title>Menu</title>
</svelte:head>

<section>
	<h1 class="text-4xl font-bold underline">Menu</h1>
	<div class="menu">
		<Button href="/game">Play</Button>
		<Button href="/scoreboard">Scoreboard</Button>
		<Button title="Med title">Knapp med titel</Button>
		<Button title="Med title" />
	</div>
</section>

<style>
	section {
		padding: 80px 0;
	}

	h1 {
		margin-bottom: 40px;
	}

	.menu {
		display: flex;
		flex-direction: column;
		align-items: center;
		margin: 0 auto;
	}
</style>
