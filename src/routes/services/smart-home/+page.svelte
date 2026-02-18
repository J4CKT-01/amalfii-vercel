<script lang="ts">
	import { Header, SmartHomeFAQ, Title } from "$lib";
    import SmartHome from "$assets/smart-thermostat.jpg";

    let services = [
        "Set and adjust the temperature of your heating system",
        "Set schedules for when your heating should be on or off",
        "Monitor the status of your boiler and get alerts if there are any issues",
        "Monitor your energy usage and receive tips for saving energy",
        "Control your heating from anywhere using a smartphone app"
    ]
</script>

<svelte:head>
    <title>Smart Home</title>
</svelte:head>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Smart Home</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Overview</Header>
                    <p class="text-xl">Smart home thermostats give you greater control over your heating system, helping you manage comfort and energy use more efficiently. With features such as programmable schedules, remote access via smartphone apps, and intelligent learning capabilities, they allow you to heat your home only when needed — reducing energy waste and lowering utility bills.
Professional installation ensures your smart thermostat integrates seamlessly with your existing boiler or heating system. Ongoing support and setup guidance help you get the most from its features, improving convenience, efficiency, and overall system performance throughout the year.</p>
                </div>
                <div class="space-y-5">
                    <img class="" src={SmartHome} alt="">
                </div>
            </div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>Benefits of a Smart Home system:</Header></div>
    <div class="grid xl:grid-cols-2 gap-5 p-6">
        {#each services as service}
        <div class="flex items-top text-2xl p-6">
            <i class="fa-sharp-duotone fa-regular fa-circle-check me-5 mt-1"></i>
            <p>{service}</p>
        </div>
        {/each}
       
    </div>
</section>

<SmartHomeFAQ />