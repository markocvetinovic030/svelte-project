<script>
	import About from '../components/about.svelte';
	import Contact from '../components/contact.svelte';
	import Footer from '../components/footer.svelte';
	import Hero from '../components/hero.svelte';
	import Introduction from '../components/introduction.svelte';
	import LinkToSvelte from '../components/linktosvelte.svelte';
	import Logo from '../components/logo.svelte';
	import PostList from '../components/postlist.svelte';
	import Tabs from '../components/shered/tabs.svelte';

	let items = ['Home', 'About', 'Contact'];
	let activeItem = 'Home';
	const tabChange = (e) => {
		activeItem = e.detail;
	};
</script>

<Logo />
<Tabs {activeItem} {items} on:tabChange={tabChange} />
{#if activeItem === 'Home'}
	<LinkToSvelte />
	<Hero />
	<Introduction />
	<PostList />
	<Footer />
{:else if activeItem === 'About'}
	<LinkToSvelte />
	<About />
	<Footer />
{:else if activeItem === 'Contact'}
	<LinkToSvelte />
	<Contact />
	<Footer />
{/if}
