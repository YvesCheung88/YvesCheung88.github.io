<script>
</script>

<nav>
	<ul class="header-menu">
		<li><a href="/">Blog</a></li>
		<li><a href="/">Portfolio</a></li>
		<li><a href="/">Contact</a></li>
		<li><a href="/">CV</a></li>
	</ul>
</nav>
<slot></slot>

<style>
	nav {
		margin-top: 30px;
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
</style>
