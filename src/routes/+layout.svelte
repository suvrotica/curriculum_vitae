<script >
	import PageHeader from '../lib/components/PageHeader.svelte';
	import Navigation from '../lib/components/Navigation.svelte';

	let links = [
		{
			href: '/',
			title: 'Home',
			image: '/Images/home.svg'
		},
		{
			href: '/about',
			title: 'About',
			image: '/Images/user.svg'
		},
		{
			href: '/contact',
			title: 'Contact',
			image: '/Images/phone.svg'
		}
	];

	let logo_image = '/Images/Logo.jpg';
</script>

<PageHeader />
<Navigation {logo_image} {links} />
<slot />

<style>
	@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200&display=swap');
</style>
