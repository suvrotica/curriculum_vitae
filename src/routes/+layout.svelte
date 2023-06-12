<script  lang="ts">

    import { onMount } from 'svelte';
    import "@picocss/pico";
    let fontLoaded = false;
  
    onMount(async () => {
      const fontLink = document.createElement("link");
      fontLink.href = "https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap";
      fontLink.rel = "stylesheet";
      document.head.appendChild(fontLink);
      fontLoaded = true;
    });
 
  

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
	:global(body) {
		font-family: 'Montserrat', sans-serif;
    font-weight: 300;
	 }
		
	
	 </style>