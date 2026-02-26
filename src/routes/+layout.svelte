<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>



<main>

<div id="a">
	<p>awdawdawdasd</p>
</div>


{@render children()}
</main>
<style>
	#a{
		background-color: yellow;
		width: 100px;
		height: 20px;
	}
	main{
		background-color: brown;
	}
	:global(body){
		background-color: aqua;
	}
</style>

