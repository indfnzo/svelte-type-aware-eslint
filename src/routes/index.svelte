<script lang="ts">
	const onClick: svelte.JSX.MouseEventHandler<HTMLButtonElement> = (evt) => {
		const object: CustomGlobalType = { id: 0, name: evt.currentTarget.innerText };
		alert(JSON.stringify(object));
	};
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<button on:click={onClick}>Click Me</button>
