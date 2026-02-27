<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>



<main>
<div id="telo">

	<div id="stranka">{@render children()}</div>
	<div id="patka">
		<div id="patka_text" class="patka_div">
			<br>Autoři: Jakub Štěpánek a Tomáš Tarábek
			<br> 2026	
		</div>
		<div id="patka_logo" class="patka_div"><img src="trebesin_logo.png" alt="Logo Třebešín"></div>

	</div>



</div>


</main>
<style>
	
	#telo{
		width: 100vw;
		max-width: 100%;
		min-height: 100vh;
		/* width: 100%;
		box-sizing: border-box;
		padding: 20px; */
		background-color: rgb(191, 191, 191);
		display: flow-root;
	}
	
	:global(body){
		background-color: aqua;
		padding: 0px;
		margin: 0px;
	}
	#patka{
		width: auto;
		height: 100px;
		background-color: #1d71b8;
		display: flex;
		gap: 10px;
		padding: 10px 25px 10px 25px;
		
		
	}
	#patka_text{
		font-size: large;
		border: 1px black solid;
		text-align: center;
		align-items: center;
		justify-content: center;
		
	}
	#patka_logo{
		border: 1px black solid;

	}
	.patka_div{
		width:100% ;
	}
</style>

