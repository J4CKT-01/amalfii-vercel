<script lang="ts">
    import {Modal, ServicePlanFAQ, Title, Header} from '$lib';
    import Fleet from '$assets/fleet.png';
    let modal1 = $state(false);
    let modal2 = $state(false);
    let modal3 = $state(false);
    let modal4 = $state(false);
    let modal5 = $state(false);
</script>
<svelte:head>
    <title>Service Plans</title>
</svelte:head>


<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Service Plans</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Overview</Header>
                    <p class="text-xl">
                        Our service plans are designed to keep your heating system safe, reliable, and running efficiently all year round — while helping you avoid unexpected repair costs. By spreading the cost monthly, you can stay on top of essential annual servicing and ongoing maintenance, protecting your boiler and heating system for the long term.
Regular servicing helps maintain manufacturer warranties where applicable and allows potential issues to be identified early, reducing the risk of costly breakdowns. With added benefits such as priority booking and discounted labour on repairs, our plans offer a simple and affordable way to maintain your home’s heating with complete peace of mind.
                    </p>
                </div>
                <div class="space-y-5">
                    <img class="" src={Fleet} alt="">
                </div>
            </div>
</section>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
            <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>Our Plans</Header></div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-5 gap-5">
                <div class="border flex flex-col p-6 space-y-10 text-center">
                    <i class="fa-sharp-duotone fa-regular fa-temperature-arrow-up text-5xl mt-6"></i>
                    <h3 class="text-2xl grow">Annual Gas Boiler</h3>
                    <div>
                        <h2 class="text-2xl font-bold underline decoration-amber-300 underline-offset-4">£9.99/Month</h2>
                        <p>(Inc. VAT)</p>
                    </div>
                    <button class="px-4 py-2 bg-amber-300" onclick={() => (modal1 = true)}>Find out more...</button>
                </div>
                <div class="border flex flex-col p-6 space-y-10 text-center">
                    <i class="fa-sharp-duotone fa-regular fa-house text-5xl mt-6"></i>
                    <h3 class="text-2xl grow">Landlord Gas Safety Inspection</h3>
                    <div>
                        <h2 class="text-2xl font-bold underline decoration-amber-300 underline-offset-4">£10.99/Month</h2>
                        <p>(Inc. VAT)</p>
                    </div>
                    <button class="px-4 py-2 bg-amber-300" onclick={() => (modal2 = true)}>Find out more...</button>
                </div>
                <div class="border flex flex-col p-6 space-y-10 text-center">
                    <div>
                        <i class="fa-sharp-duotone fa-regular fa-temperature-arrow-up text-5xl mt-6"></i>
                        <i class="fa-sharp-duotone fa-regular fa-slash-forward text-5xl mt-6"></i>
                        <i class="fa-sharp-duotone fa-regular fa-fire text-5xl mt-6"></i>
                    </div>
                    <h3 class="text-2xl grow">Annual Gas Boiler and Gas Fire</h3>
                    <div>
                        <h2 class="text-2xl font-bold underline decoration-amber-300 underline-offset-4">£13.99/Month</h2>
                        <p>(Inc. VAT)</p>
                    </div>
                    <button class="px-4 py-2 bg-amber-300" onclick={() => (modal3 = true)}>Find out more...</button>
                </div>
                <div class="border flex flex-col p-6 space-y-10 text-center">
                    <i class="fa-sharp-duotone fa-regular fa-air-conditioner text-5xl mt-6"></i>
                    <h3 class="text-2xl grow">Air Source Heat Pump Basic Service</h3>
                    <div>
                        <h2 class="text-2xl font-bold underline decoration-amber-300 underline-offset-4">£13.99/Month</h2>
                        <p>(Inc. VAT)</p>
                    </div>
                    <button class="px-4 py-2 bg-amber-300" onclick={() => (modal4 = true)}>Find out more...</button>
                </div>
                <div class="border flex flex-col p-6 space-y-10 text-center col-span-1 md:col-span-2 lg:col-span-1">
                    <div>
                        <i class="fa-sharp-duotone fa-regular fa-house text-5xl mt-6"></i>
                        <i class="fa-sharp-duotone fa-regular fa-slash-forward text-5xl mt-6"></i>
                        <i class="fa-sharp-duotone fa-regular fa-vent-damper text-5xl mt-6"></i>
                    </div>
                    <h3 class="text-2xl grow">Air Source Heat Pump and System</h3>
                    <div>
                        <h2 class="text-2xl font-bold underline decoration-amber-300 underline-offset-4">£19.99/Month</h2>
                        <p>(Inc. VAT)</p>
                    </div>
                    <button class="px-4 py-2 bg-amber-300" onclick={() => (modal5 = true)}>Find out more...</button>
                </div>
            </div>
            <div class="w-full flex justify-start lg:justify-center"><p class="self-center w-full lg:w-1/3">all service plans come with 15% labour discount (if repairs are required), certificates and yearly reminders. <a href="/service-plans-terms-and-conditions" class="underline">terms and conditions apply</a></p></div>
		</div>
        
	</div>
</section>

<Modal bind:showModal={modal1}>
    {#snippet header()}
        <h3 class="text-4xl">Includes:</h3>
        <p class="text-xl">An annual inspection and service of a single boiler in the plan holders own property. as well as:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1">
        <li>Carbon monoxide monitor testing</li>
        <li>Smoke alarm testing</li>
        <li>Gas meter check and testing</li>
    </ul>
    <p>One off service cost: £85 + VAT</p>
</Modal>

<Modal bind:showModal={modal2}>
    {#snippet header()}
        <h3 class="text-4xl">Includes:</h3>
        <p class="text-xl">an annual inspection and service of a single boiler in the plan holders property and a visual inspection of other gas appliances in the same property. as well as:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1">
        <li>Carbon monoxide monitor testing</li>
        <li>Smoke alarm testing</li>
        <li>Gas meter check and testing</li>
        <li>CP12 Produced and date managed.</li>
    </ul>
    <p>Remember: Having a valid CP12 in a rental property is a legal requirement.</p>
    <p>One off service cost: £85 + VAT</p>
</Modal>

<Modal bind:showModal={modal3}>
    {#snippet header()}
        <h3 class="text-4xl">Includes:</h3>
        <p class="text-xl">an annual inspection and service of a single boiler and single gas fire in the plan holders property. as well as:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1">
        <li>Carbon monoxide monitor testing</li>
        <li>Smoke alarm testing</li>
        <li>Gas meter check and testing</li>
    </ul>
    <p>One off service cost: £125 + VAT</p>
</Modal>

<Modal bind:showModal={modal4}>
    {#snippet header()}
        <h3 class="text-4xl">Includes:</h3>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1">
        <li>Checking outdoor unit</li>
        <li>Checking antifreeze</li>
        <li>Cleaning filter</li>
        <li>Checking and cleaning fans</li>
        <li>Removal of trapped hair</li>
        <li>Pressures checked</li>
        <li>Checking flow rate and adjust if necessary</li>
        <li>Checking and optimising controller settings</li>
        <li>Paperwork completed</li>
    </ul>
    <p>One off service cost: £150 inc VAT</p>
</Modal>

<Modal bind:showModal={modal5}>
    {#snippet header()}
        <h3 class="text-4xl">Includes:</h3>
        <p class="text-xl">All services in the Air Source Heat Pump Service Plan, as well as:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1">
        <li>Checking immersion heater function</li>
        <li>Cleaning evaporator fans and comb straight</li>
        <li>Checking insulation</li>
        <li>Checking expansion vessel, pressure and air unit</li>
        <li>Checking for leaks of water and refrigerant</li>
        <li>Servicing hot water cylinder, testing correct operation of all safety components</li>
        <li>Checking Electrical supply, condition and operation</li>
        <li>Checking refrigerant pressures and heatline temperatures</li>
        <li>Checking for fault codes on control unit</li>
        <li>Paperwork Completed</li>
    </ul>

    <p>One off service cost: £240 + VAT</p>
</Modal>
<ServicePlanFAQ />