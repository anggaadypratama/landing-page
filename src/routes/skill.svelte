<script>
	import Skill from '../components/local/skill/Skill.svelte'
	import Galery from '../components/local/skill/Galery.svelte';

</script>

<svelte:head>
	<title>Skill & Experience</title>
</svelte:head>

<div class="grid grid-cols-1 grid-rows-2 md:grid-rows-1 md:grid-cols-2 gap-0 md:mt-0 mt-16">
	<Skill className="px-4 relative"/>
	<Galery/>
</div>
