<script >
	export let links;
	export let logo_image;
</script>

<nav>
	<div><img src={logo_image} width="50%" alt="Suvro Ghosh Logo" /></div>
	<ul>
		{#each links as link}
			<li><span><img src={link.image} alt={link.title}></span><a href={link.href} title={link.title}>{link.title}</a></li>
		{/each}
	</ul>
</nav>

<style>



    nav {
        margin:auto;
        width: 80%;
    }

    a {
        color: black;
		font-size: 18px;
        text-transform: uppercase;
    }

    

    li img{
        vertical-align: middle;
        margin-right: 10px;
    }
   
	/* Hover effect */
	a:hover::before {
		content: attr(title);
		position: absolute;
		background-color: black;
		color: white;
		padding: 4px 8px;
		border-radius: 4px;
		font-size: 18px;
        text-transform: uppercase;
		visibility: hidden;
		opacity: 0;
		transition: visibility 0s, opacity 0.2s linear;
	}

	a:hover:hover::before {
		visibility: visible;
		opacity: 1;
	}
</style>
