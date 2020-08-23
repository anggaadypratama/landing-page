<script>
	import Home from '../components/local/home/Home.svelte'

</script>

<svelte:head>
	<title>Angga Ady Pratama</title>
</svelte:head>

<div class="grid grid-cols-1 grid-rows-2 md:grid-rows-1 md:grid-cols-2 gap-0 md:mt-0 mt-16">
	<Home className="px-4 relative"></Home>
	<div class="i">9</div>
</div>

<style lang="scss">
	@import '../../static/style/global.scss';

	@media screen and (min-width: $md){
	.i{
		min-height: 960px;
        width: 100%;
        display: inline;
        background-color: aliceblue;
	
	}
}
</style>