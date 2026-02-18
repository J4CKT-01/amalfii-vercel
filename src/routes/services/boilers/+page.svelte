<script lang="ts">
	import { BoilerFAQ, Header, Title } from "$lib";
    import Boiler from "$assets/boiler.jpg";
</script>

<svelte:head>
    <title>Boilers</title>
</svelte:head>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Boilers</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Overview</Header>
                    <p class="text-xl">Your boiler is the heart of your heating system, providing reliable warmth and hot water throughout the year. Choosing the right boiler and ensuring professional installation helps improve energy efficiency, reduce running costs, and deliver consistent performance for your property.
Routine servicing is essential to keep your boiler operating safely and efficiently. Regular inspections help identify potential issues early, prevent unexpected breakdowns, and extend the lifespan of your system. If a problem does arise, prompt and professional repairs can quickly restore heating and hot water, minimising disruption and keeping your home or business comfortable.</p>
                </div>
                <div class="space-y-5">
                    <img class="" src={Boiler} alt="">
                </div>
            </div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
        <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>What we offer:</Header></div>
            <div class="grid xl:grid-cols-3 gap-10 *:border">
                <div class="p-6 space-y-5">
                    <div class="text-center"><i class="fa-sharp-duotone fa-regular fa-toolbox text-5xl"></i></div>
                    <div class="h-30 flex justify-center"><Header>Services</Header></div>
                    <p class="text-xl">
                        Regular boiler servicing is essential to keep your heating system operating safely, efficiently, and reliably throughout the year. We recommend an annual service to help prevent unexpected breakdowns and maintain optimal performance. Our Gas Safe registered engineers are experienced in servicing all makes and models of gas boilers, carrying out thorough inspections, cleaning key components, and checking safety controls. Routine servicing not only improves energy efficiency and extends the lifespan of your boiler, but also helps identify potential issues early — reducing the risk of costly repairs and ensuring continued peace of mind.
                    </p>
                </div>
                <div class="p-6 space-y-5">
                    <div class="text-center"><i class="fa-sharp-duotone fa-regular fa-toolbox text-5xl"></i></div>
                    <div class="h-30 flex justify-center"><Header>Repairs</Header></div>
                    <p class="text-xl">
                        If your boiler develops a fault or stops working altogether, our Gas Safe heating engineers are ready to respond quickly and efficiently. We diagnose and repair a wide range of common issues, including faulty thermostats, low pressure, leaking or frozen pipes, ignition failures, and malfunctioning pumps or valves. Our team carefully inspects essential components such as the heat exchanger, controls, and safety devices to pinpoint the cause of the problem. By delivering thorough, professional repairs, we restore heat and hot water as quickly as possible, ensuring your home or business returns to full comfort with minimal disruption.
                    </p>
                </div>
               <div class="p-6 space-y-5">
                    <div class="text-center"><i class="fa-sharp-duotone fa-regular fa-toolbox text-5xl"></i></div> 
                    <div class="h-30 flex justify-center **:text-center"><Header>Central Heating Installation & Maintenance</Header></div>
                    <p class="text-xl">Whether you’re installing a new central heating system or upgrading an existing one, our experienced engineers deliver a reliable and efficient service tailored to your property. We install boilers, radiators, pipework, and heating controls to ensure balanced heat distribution and dependable performance throughout your home or business.
We also provide ongoing maintenance and repairs to keep your system running at its best. From identifying circulation issues and leaks to checking controls and system pressure, we help prevent breakdowns and ensure consistent, energy-efficient comfort all year round.</p>
                </div> 
            </div>
</section>

<BoilerFAQ />