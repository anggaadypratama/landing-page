<script>
	import Tailwindcss from '../components/Tailwindcss.svelte';
	import Nav from '../components/Nav.svelte';

	export let segment;
</script>

<style lang="scss">
	@import '../../static/style/global.scss';

	:global(body){
		background-color: $primary;
	}

	main {
		color: white;
	}

</style>

<Tailwindcss />

<Nav {segment}/>

<main class="">
	<div class="md:ml-16">
		<slot></slot>
	</div>
</main>