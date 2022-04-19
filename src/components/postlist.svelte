<script>
	import { onMount } from 'svelte';

	let posts = [];

	onMount(async () => {
		const response = await fetch('https://jsonplaceholder.typicode.com/posts');
		posts = await response.json();
		console.log(posts);
	});
</script>

<div class="p-10 bg-gray-50 pb-40">
	<p class="font-bold text-5xl text-orange-500 mb-40 mt-10 text-center">Posts</p>
	<div class=" overflow-y-scroll bg-gray-50 w-8/12 h-96 m-auto p-10 border-2 border-gray-200 ">
		{#each posts as post (post.id)}
			<h3 class="text-xl text-center mb-4 mt-4 text-orange-500 font-bold">
				{post.id}. {post.title}
			</h3>
			<p class="text-orange-500 text-center pl-20 pr-20 mb-6">{post.body}</p>
			<hr />
		{:else}
			<p>Loading...</p>
		{/each}
	</div>
</div>
