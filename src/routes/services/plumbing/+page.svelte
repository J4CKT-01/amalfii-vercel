<script lang="ts">
	import { Header, PlumbingFAQ, Title } from "$lib";
    import Plumbing from "$assets/plumbing.jpg";

    let services = [
        "Water leak repairs", "New pipe installation and repair",
        "Toilet repair and replacement", "Tap repair and replacement",
        "Hot water cylinder repair and installation", "Vented and unvented systems",
        "Water treatments", "Shower repair and installation", "Stopcock repair",
        "Radiator installation, repair or replacement", "Radiator valve fit, repair or replacement"
    ]
</script>

<svelte:head>
    <title>Plumbing</title>
</svelte:head>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Plumbing</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Overview</Header>
                    <p class="text-xl">A reliable plumbing system is essential for the smooth running of any home or business, delivering clean water and effective drainage every day. From new installations to upgrades and replacements, professional plumbing work ensures your system operates efficiently, safely, and in line with current standards.
Regular maintenance and timely repairs help prevent leaks, water damage, and costly disruptions. Whether it’s resolving pipework issues, repairing fixtures, or addressing drainage concerns, prompt and professional service keeps your plumbing system performing reliably and protects your property for the long term.</p>
                </div>
                <div class="space-y-5">
                    <img class="" src={Plumbing} alt="">
                </div>
            </div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>Common Plumbing services include:</Header></div>
    <div class="grid xl:grid-cols-3 gap-5 p-6">
        {#each services as service}
        <div class="flex items-top text-2xl p-6">
            <i class="fa-sharp-duotone fa-regular fa-circle-check me-5 mt-1"></i>
            <p>{service}</p>
        </div>
        {/each}
       
    </div>
</section>

<PlumbingFAQ />