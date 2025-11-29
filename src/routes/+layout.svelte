<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header>
	<a href="/">
		<h3>🐇 Find my Förderung</h3>
	</a>
</header>
<nav>
	<ul>
		<li><a href="/">Home</a></li>
		<li><a href="/find-my-foerderung">Find my Förderung</a></li>
		<li><a href="/application-wizard">Application Wizard</a></li>
		<li><a href="/data-room">Stakeholder Data Room</a></li>
		<li><a href="/auth">Login / SignUp</a></li>
	</ul>
</nav>

{@render children()}

<style>
	header {
		background-color: #f0f0f0;
		padding: 1rem;
	}
	nav {
		background-color: #f0f0f0;
		padding: 1rem;
	}
	ul {
		list-style: none;
		padding: 0;
	}
	li {
		display: inline-block;
		margin-right: 1rem;
	}
	a {
		text-decoration: none;
		color: #333;
	}
	a:hover {
		color: #000;
	}
</style>