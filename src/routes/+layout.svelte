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
	import GasSafe from '$assets/gassafe.png';
	import type { Attachment } from 'svelte/attachments';

	let { children } = $props()

	let menuopen = $state(false);
	let servicemenuopen = $state(false);
	let surveymenuopen = $state(false);
	let top = $state(0), left = $state(0);

	function setDropdownPosition(element: HTMLElement) {
		const rect = element.getBoundingClientRect();
		top = rect.bottom;
		left = rect.left;

	$effect(() => {
		if (!servicemenuopen) {
			surveymenuopen = false;
		}
	})
	}
</script>
<!-- Nav Container -->
<nav class="container mx-auto">
	<!-- Nav Flex Box -->
	 <div class="flex items-center justify-between">
		<!-- Logo -->
		<button onclick={() => goto("/")} class="flex hover:cursor-pointer" aria-label="Go to Homepage"><img class="size-24" src={logo} alt="amalfii logo"></button>
		<!-- Menu Buttons -->
		<div class="hidden lg:flex justify-evenly text-2xl">
			<a href="/" class="{page.route.id === "/" ? "bg-amber-300" : " "} py-4 px-15 ">Home</a>
			<div class="relative">
				<button {@attach setDropdownPosition} onclick={() => servicemenuopen = !servicemenuopen}
					class="{page.route.id.includes("/service") ? "bg-amber-300" : " "} py-4 px-15 hover:cursor-pointer"
					>Our Services</button>
					{#if servicemenuopen}
				<div class="absolute flex flex-col gap-0.5 shadow-md bg-white left-0 top-full w-100">
					<a href="/services/service-plans" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/service-plans" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Service Plans</a>
					<a href="/services/plumbing" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/plumbing" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Plumbing</a>
					<a href="/services/boilers" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/boilers" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Boilers</a>
					<a href="/services/air-source-heat-pumps" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/air-source-heat-pumps" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Air Source Heat Pumps</a>
					<button href="/services/surveys" onclick={() => {surveymenuopen = !surveymenuopen;}} class="{page.route.id.startsWith("/services/surveys") ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15 items-center flex hover:cursor-pointer">Surveys <span class="ms-5"><i class="fa-sharp-duotone fa-regular fa-caret-right"></i></span></button>
					{#if surveymenuopen}
					<a href="/services/surveys/pre-purchase-plumbing-and-heating" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/surveys/pre-purchase-plumbing-and-heating" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Pre-Purchase Plumbing & Heating</a>
					<a href="/services/surveys/air-source-heat-pumps-suitability" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/surveys/air-source-heat-pumps-suitability" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15 border-b">Air Source Heat Pump Suitability</a>
					{/if}
					<a href="/services/smart-home" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/smart-home" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Smart Home</a>
				</div>
			{/if}
			</div>
			<a href="/contact" class="{page.route.id === "/contact" ? "bg-amber-300" : " "} py-4 px-15">Contact</a>
		</div>
	<!-- Dropdown Button -->
	<div class="flex lg:hidden text-2xl">
		<button aria-label="menu" onclick={() => menuopen = !menuopen} class="h-full {menuopen ? "bg-amber-300" : " "} py-4 px-15 "><i class="fa-sharp-duotone fa-regular fa-bars"></i></button>
	</div>
	<!-- Dropdown Menu -->
	</div>
	<div class="{menuopen ? "flex" : "hidden"} flex-col lg:hidden justify-evenly text-2xl text-center">
		<a href="/" onclick={() => menuopen = false} class="{page.route.id === "/" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Home</a>
		<button aria-label="menu" onclick={() => servicemenuopen = !servicemenuopen} class="{servicemenuopen ? "bg-amber-300" : " "} py-4 px-15 ">Our Services <i class="fa-sharp-duotone fa-regular fa-caret-right"></i></button>
		<div class="{servicemenuopen ? "flex" : "hidden"} flex-col justify-evenly text-2xl text-center shadow-xl">
			<a href="/services/plumbing" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/plumbing" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Plumbing</a>
			<a href="/services/boilers" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/boilers" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Boilers</a>
			<a href="/services/air-source-heat-pumps" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/air-source-heat-pumps" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Air Source Heat Pumps</a>
			<button href="/services/surveys" onclick={() => {surveymenuopen = !surveymenuopen;}} class="{page.route.id.startsWith("/services/surveys") ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15 items-center flex justify-center hover:cursor-pointer">Surveys <span class="ms-2"><i class="fa-sharp-duotone fa-regular fa-caret-right"></i></span></button>
				{#if surveymenuopen}
				<a href="/services/surveys/pre-purchase-plumbing-and-heating" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/surveys/pre-purchase-plumbing-and-heating" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Pre-Purchase Plumbing & Heating</a>
				<a href="/services/surveys/air-source-heat-pumps-suitability" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/surveys/air-source-heat-pumps-suitability" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15 border-b">Air Source Heat Pump Suitability</a>
				{/if}
			<a href="/services/smart-home" onclick={() => {servicemenuopen = false; menuopen = false}} class="{page.route.id === "/services/smart-home" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Smart Home</a>
		</div>
		<a href="/contact" onclick={() => menuopen = false} class="{page.route.id === "/contact" ? "bg-amber-300 underline" : " "} hover:underline py-4 px-15">Contact</a>
	</div>
</nav>

<div class="fixed bottom-0 right-0 p-6 z-10">
	<a href="/#company-info"><img class="size-16 lg:size-32 object-fill" src={GasSafe} alt="gas safe logo" aria-label="Gas Safe Link"></a>
</div>
{@render children()}

<div class="container mt-5 lg:mt-15 mx-auto flex flex-col p-2 lg:p-6 lg:flex-col">
	<div class="flex flex-row min-h-min space-x-10">
		<div>
			<img src={ovo} alt="ovo logo">
		</div>
		<div>
			<img src={refcom} alt="refcom logo">
		</div>
		<div>
			<img src={glowgreen} alt="glowgreen logo">
		</div>
		<div>
			<img src={hometree} alt="hometree logo">
		</div>
		<div>
			<img src={verysmart} alt="very smart home company logo">
		</div>
		<div>
			<img src={boxt} alt="boxt logo">
		</div>

		<div>
			<img src={yourrepair} alt="your repair logo">
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
		<p>Amalfii Heating ©x-2024 All Rights Reserved. <a class="underline" href="/terms-and-conditions">Privacy Policy</a></p>
	</div>
</footer>
