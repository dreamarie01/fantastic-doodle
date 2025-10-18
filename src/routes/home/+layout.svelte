<script>
	import '../../app.css';
	import favicon from '$lib/assets/favicon.svg';
    import Button from '$lib/components/ui/button/button.svelte';
    

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="headWrapper flex">
    <Button href="/" variant="link">Landing</Button>
    <Button href="/home" variant="link">Home</Button>
</div>

{@render children?.()}