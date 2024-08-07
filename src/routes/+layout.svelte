<script>
	import ThemeController from '$lib/component/ThemeController.svelte';
	import '../app.css';
</script>

<nav>
	<ul class="header-menu">
		<li><a href="/Blog">Blog</a></li>
		<li><a href="/Portfolio">Portfolio</a></li>
		<li><a href="/Contact">Contact</a></li>
		<li><a href="/CV">CV</a></li>
		<li class="theme-controller-wrapper">
			<ThemeController />
		</li>
	</ul>
</nav>
<slot></slot>

<style>
	nav {
		margin: 30px;
	}
	.header-menu {
		display: flex;
		list-style: none;
		gap: 10px;
		font-size: 32px;
		font-weight: bold;

		& a {
			text-decoration: none;
			cursor: pointer;
			color: black;
			padding: 5px;
		}
	}
	.header-menu a:hover {
		background-color: blue;
	}
	.theme-controller-wrapper {
		margin-left: auto;
	}
</style>
