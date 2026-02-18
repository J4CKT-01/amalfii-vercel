<script lang="ts">
	import { ASHPFAQ, Header, Title } from "$lib";
    import ASHP from "$assets/ashp.jpg";

    let services = [
        "Lower your energy bills", "Cut your carbon footprint",
        "Raise your property value", "Easier to maintain than combustion systems",
        "Often include warranties of up to 7 years"]
</script>

<svelte:head>
    <title>Air Source Heat Pumps</title>
</svelte:head>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Air Source Heat Pumps</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="grid xl:grid-cols-2 gap-10">
        <div class="p-6 space-y-5">
            <Header>Overview</Header>
            <p class="text-xl">
                A reliable plumbing system is essential for the smooth running of any home or business, delivering clean water and effective drainage every day. From new installations to upgrades and replacements, professional plumbing work ensures your system operates efficiently, safely, and in line with current standards.
Regular maintenance and timely repairs help prevent leaks, water damage, and costly disruptions. Whether it’s resolving pipework issues, repairing fixtures, or addressing drainage concerns, prompt and professional service keeps your plumbing system performing reliably and protects your property for the long term.
            </p>
        </div>
        <div class="space-y-5">
            <img class="" src={ASHP} alt="">
        </div>
    </div>
</section>


<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>Benefits of Air Source Heat Pumps:</Header></div>
    <div class="grid xl:grid-cols-3 gap-5 p-6">
        {#each services as service}
        <div class="flex items-top text-2xl p-6">
            <i class="fa-sharp-duotone fa-regular fa-circle-check me-5 mt-1"></i>
            <p>{service}</p>
        </div>
        {/each}
       
    </div>
</section>

<ASHPFAQ />