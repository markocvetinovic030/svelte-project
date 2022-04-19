<script>
	import About from '../components/about.svelte';
	import Footer from '../components/footer.svelte';
	import Introduction from '../components/introduction.svelte';
	import LinkToSvelte from '../components/linktosvelte.svelte';
	import PostList from '../components/postlist.svelte';
	import Tabs from '../components/shered/tabs.svelte';

	let items = ['Home', 'About', 'Contact'];
	let activeItem = 'Home';
	const tabChange = (e) => {
		activeItem = e.detail;
	};
</script>

<Tabs {activeItem} {items} on:tabChange={tabChange} />
{#if activeItem === 'Home'}
	<LinkToSvelte />
	<Introduction />
	<PostList />
	<Footer />
{:else if activeItem === 'About'}
	<About />
	<Footer />
{:else if activeItem === 'Contact'}
	<p>car</p>
{/if}
