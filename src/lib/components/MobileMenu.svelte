<script lang="ts">
	import {mobileMenuOpen} from "../../stores/store"
	import NavLinks from "./NavLinks.svelte";
	import Close from "./icons/Close.svelte";
</script>

<div
	class={`${
		$mobileMenuOpen ? 'top-0' : 'top-[-100%]'
	} font-semibold fixed w-full shadow-lg transition-all duration-[.7s] ease-out left-0 right-0 bg-black p-8 overflow-auto z-[1000] h-full`}
>
	<button on:click={() => mobileMenuOpen.set(false)}>
		<Close class="text-4xl" />
	</button>
	<nav class="list-none grid justify-center mt-10 text-center text-xl font-bold gap-16">
		<NavLinks		
			links={[
				{ name: 'Home', url: '/' },
				{ name: 'About', url: '#about' },
				{ name: 'GIF Winners List 2024', url: '#winners-list' },
				{ name: 'Services', url: '#services' },
				{ name: 'Contact', url: '#contact' }
			]}
		/>
	</nav>
</div>
