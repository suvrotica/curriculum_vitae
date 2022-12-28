<script>
	export let links;
</script>

<nav>
	<ul>
		<li>
			<strong>Curriculum Vitae</strong>
			<cite> - Suvro Ghosh</cite>
		</li>
	</ul>
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

	cite {
		font-weight: 100;
	}

	strong {
		font-weight: 200;
		text-transform: uppercase;
	}
	nav {
		margin: auto;
		width: 95%;
		
	}

	a {
		font-weight: 200;
		text-transform: uppercase;
		text-decoration: none;
	}

	li img {
		vertical-align: middle;
		margin-right: 10px;
	}
</style>
