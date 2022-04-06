<script lang="ts">
	export let title: string = undefined;
	export let href: string = undefined;

	const handleClick = console.log;
</script>

{#if !!href}
	<a {title} {href}><slot /></a>
{:else}
	<button {title} on:click={handleClick}><slot /></button>
{/if}

<style>
	button,
	a {
		width: 100%;
		max-width: 480px;
		height: 50px;

		margin: 1rem 0;

		line-height: 50px;
		font-size: 1.5rem;
		font-weight: bold;
		text-align: center;
		text-decoration: none;

		color: black;
		border: 1px solid gray;
	}
	a:hover,
	button:hover {
		text-decoration: none;
	}
</style>
