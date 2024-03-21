<script lang="ts">
	import { mobileMenuOpen } from '../../stores/store';
	export let links: Array<{ name: string; url: string }>;
	export let className: string | undefined = undefined
</script>

<ul class={className ?? ""}>
	{#each links as link}
		<li>
			<a href={link.url} on:click={() => mobileMenuOpen.set(false)}>{link.name}</a>
		</li>
	{/each}
</ul>
