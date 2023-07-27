<script lang="ts">
	import Card from '../components/Card.svelte'
	const content_list = [
		{
			main_content: "Basic",
		},
		{
			main_content: "WE",
		},
		{
			main_content: "trim",
		},
		{
			main_content: "Basic",
		},
		{
			main_content: "WE",
		},
		{
			main_content: "trim",
		},
		{
			main_content: "Basic",
		},
		{
			main_content: "WE",
		},
		{
			main_content: "trim",
		}
	]
</script>

<div class="flex w-4/5 flex-wrap m-auto justify-center py-10">
	{#each content_list as content,index}
		<Card main_content={content.main_content} index={index}/>
	{/each}
</div>