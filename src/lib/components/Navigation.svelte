<script>
	export let links;
	export let logo_image;
</script>

<nav>
	<div><img src={logo_image} width="50%" alt="Suvro Ghosh Logo" /></div>
	<ul>
		{#each links as link}
			<li>
				<span><img src={link.image} alt={link.title} /></span><a
					href={link.href}
					title={link.title}>{link.title}</a
				>
			</li>
		{/each}
	</ul>
</nav>

<style>
	nav {
		margin: auto;
		width: 80%;
	}

	a {
		text-transform: uppercase;
	}

	li img {
		vertical-align: middle;
		margin-right: 10px;
	}
</style>
