<script>
	import '../app.postcss';
	import { Navbar, NavBrand, NavHamburger, NavLi, NavUl } from 'flowbite-svelte';
	import { TerminalSolid } from 'flowbite-svelte-icons';
</script>

<Navbar>
	<NavBrand href="/">
		<TerminalSolid class="mr-2" size="lg" alt="Content Platform Logo" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
			Content Platform
		</span>
	</NavBrand>
	<NavHamburger />
	<NavUl>
		<NavLi href="/">Home</NavLi>
		<NavLi href="/login">Log in</NavLi>
		<NavLi href="/about">About</NavLi>
	</NavUl>
</Navbar>
<div class="p-8">
	<slot />
</div>
