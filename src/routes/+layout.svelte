<script lang="ts">
	import logo from '$assets/logo.png';
    import ovo from "$assets/ovo.png";
    import refcom from "$assets/refcom.png";
    import glowgreen from "$assets/gg.png";
    import hometree from "$assets/ht.png";
    import verysmart from "$assets/tvshc.png";
    import boxt from "$assets/boxt.png";
    import yourrepair from "$assets/yr.png";
	import { page } from '$app/state';
	import '../app.css';
	import { goto } from '$app/navigation';
	let { children } = $props()
	let menuopen = $state(false);
	$inspect(menuopen);
</script>

<!-- Nav Container -->
<nav class="container mx-auto">
	<!-- Nav Flex Box -->
	 <div class="flex items-center justify-between">
		<!-- Logo -->
		<button onclick={() => goto("/")} class="flex hover:cursor-pointer"><img class="size-24" src={logo} alt=""></button>
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

<div class="container mt-5 lg:mt-15 mx-auto flex flex-col p-2 lg:p-6 lg:flex-col">
	<div class="flex flex-row min-h-min space-x-10">
		<div>
			<img src={ovo} alt="">
		</div>
		<div>
			<img src={refcom} alt="">
		</div>
		<div>
			<img src={glowgreen} alt="">
		</div>
		<div>
			<img src={hometree} alt="">
		</div>
		<div>
			<img src={verysmart} alt="">
		</div>
		<div>
			<img src={boxt} alt="">
		</div>

		<div>
			<img src={yourrepair} alt="">
		</div>
	</div>
</div>
<!-- Footer -->
<footer class="bg-amber-300 w-full">
	<!-- Footer Flex Box -->
	<div class="container flex flex-col lg:flex-row items-center  mx-auto text-xl">
		<div class="py-8 w-1/2 text-lg space-x-10 justify-center flex flex-row text-center">
			<a class="hover:underline" href="/">Home</a>
			<a class="hover:underline" href="/services">Services and Pricing</a>
			<a class="hover:underline" href="/contact">Contact</a>
		</div>
		<div id="company-info" class="py-8 text-sm w-1/2 space-x-5 flex flex-col text-center">
			<p>Company No: 1164596</p>
			<p>VAT Reg: 353488671</p>
			<p>Gas Safe No: 625151</p>
			<p>Reg Office: Office 7, The Civic Centre,</p>
			<p>Martins Way, Stourport-on-Severn, DY13 8UN</p>
		</div>
	</div>
	<div class="w-full text-center py-3 text-gray-600">
		<p>Amalfii Heating ©x-2024 All Rights Reserved. <a class="underline" href="/terms-and-conditions">Terms of Use</a> and <a class="underline" href="/terms-and-conditions">Privacy Policy</a></p>
	</div>
</footer>
