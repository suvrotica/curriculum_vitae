<script>
	import Navigation from "../lib/components/Navigation.svelte";

	let links = [
		{
			href: "/",
			title: "Home",
			image: "/Images/home.svg",
		},
		{
			href: "/about",
			title: "About",
			image: "/Images/user.svg",
		},
		{
			href: "/contact",
			title: "Contact",
			image: "/Images/phone.svg",
		},
		{
			href: "/Images/download.svg",
			title: "CV",
			image: "/Images/download.svg",
		}
	];

</script>

<header>
	<Navigation {links} />
</header>

<slot />

<style>
	@import url("https://unpkg.com/@picocss/pico@latest/css/pico.classless.min.css");
	@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200&display=swap");
</style>
