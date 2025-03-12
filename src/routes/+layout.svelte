<script lang="ts">
	import logo from '$assets/logo.png';
	import { page } from '$app/state';
	import '../app.css';
	let { children } = $props()
	let menuopen = $state(false);
	$inspect(menuopen);
</script>

<!-- Nav Container -->
<nav class="container mx-auto">
	<!-- Nav Flex Box -->
	 <div class="flex items-center justify-between">
		<!-- Logo -->
		<div class="flex"><img class="size-16" src={logo} alt=""></div>
		<!-- Menu Buttons -->
		<div class="hidden lg:flex justify-evenly text-2xl">
			<a href="/" class="{page.route.id === "/" ? "bg-amber-300" : " "} py-4 px-15 ">Home</a>
			<a href="/services" class="{page.route.id === "/services" ? "bg-amber-300" : " "} py-4 px-15">Services and Pricing</a>
			<a href="/contact" class="{page.route.id === "/contact" ? "bg-amber-300" : " "} py-4 px-15 ">Contact</a>
		</div>
	<!-- Dropdown Button -->
	<div class="flex lg:hidden text-2xl">
		<button aria-label="menu" onclick={() => menuopen = !menuopen} class="h-full {menuopen ? "bg-amber-300" : " "} py-4 px-15 "><i class="fa-sharp-duotone fa-regular fa-bars"></i></button>
	</div>
	<!-- Dropdown Menu -->
	</div>
	<div class="{menuopen ? "flex" : "hidden"} flex-col lg:hidden justify-evenly text-2xl text-center">
		<a href="/" onclick={() => menuopen = false} class="{page.route.id === "/" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Home</a>
		<a href="/services" onclick={() => menuopen = false} class="{page.route.id === "/services" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Services and Pricing</a>
		<a href="/contact" onclick={() => menuopen = false} class="{page.route.id === "/contact" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Contact</a>
	</div>
</nav>


{@render children()}

<!-- Footer -->
<footer class="bg-amber-300 w-full">
	<!-- Footer Flex Box -->
	<div class="container flex flex-col lg:flex-row items-center  mx-auto text-xl">
		<!-- Social Icons -->
		<!-- <div class="py-6 w-full lg:w-1/2 flex justify-center text-2xl">
			<i class="fa-sharp-duotone fa-regular fa-thumbs-up"></i>
			<i class="fa-sharp-duotone fa-regular fa-thumbs-up px-40"></i>
			<i class="fa-sharp-duotone fa-regular fa-thumbs-up"></i>
		</div> -->
		<div class="py-6 w-full flex justify-evenly">
			<a class="" href="/">Home</a>
			<a class="px-15" href="/services">Services and Pricing</a>
			<a class="" href="/contact">Contact</a>
		</div>
	</div>
	<div class="w-full text-center py-4 text-gray-600">
		<p>Amalfii Heating ©x-2024 All Rights Reserved. <a class="underline" href="/terms-and-conditions">Terms of Use</a> and <a class="underline" href="/terms-and-conditions">Privacy Policy</a></p>
	</div>
</footer>
