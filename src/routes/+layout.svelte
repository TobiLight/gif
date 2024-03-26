<script lang="ts">
	import '../app.css';
	import Menu from '$lib/components/icons/Menu.svelte';
	import MobileMenu from '../lib/components/MobileMenu.svelte'
	import NavLinks from '$lib/components/NavLinks.svelte';
	import {mobileMenuOpen} from "../stores/store"

</script>

<svelte:head>
	<title>Global Innovation Fund 2024</title>
</svelte:head>

<header class="flex fixed z-[9999] top-0 w-full justify-between gap-4 items-center p-4 bg-black text-white">
	<button class="md:hidden" on:click={() => mobileMenuOpen.set(true)}>
		<Menu class="text-2xl" />
	</button>
	
	<div class="logo mx-auto md:mx-0 text-center">
		<h1 class="font-bold break-words">GLOBAL INNOVATION FUND</h1>
	</div>

	<MobileMenu />

	<div class="hidden md:block">
		<nav>
			<NavLinks
			className="flex justify-between list-none gap-6"
				links={[
					{ name: 'Home', url: '/' },
					{ name: 'About', url: '#about' },
					{ name: 'GIF Winners List 2024', url: '#winners-list' },
					// { name: 'Services', url: '#services' },
					{ name: 'Contact', url: '#contact' }
				]}
			/>
		</nav>
	</div>
</header>
<main class="min-h-screen mt-[3.5rem]">
	<slot />
</main>
<footer class="bg-black p-8 text-white">
	<div class="flex flex-col gap-4 items-center">
		<nav>
			<NavLinks className="flex gap-4 items-center list-none flex-wrap justify-center" links={[
					{ name: 'Home', url: '/' },
					{ name: 'About', url: '#about' },
					{ name: 'GIF Winners List 2024', url: '#winners-list' },
					{ name: 'Services', url: '#services' },
					{ name: 'Contact', url: '#contact' }
				]} />
		</nav>
		<div>
			<h1>GLOBAL INNOVATION FUND</h1>
			<p class="text-xs">Copyright © 2024 All rights reserved</p>
		</div>
	</div>
</footer>
