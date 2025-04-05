<script lang="ts">
	import { Modal } from '$lib';
    import ASHPImage from '$assets/ashp.jpg.avif';
    import SmartThermoImage from '$assets/smart-thermostat.jpg.avif';
    import PlumbingImage from '$assets/plumbing.jpg.avif';
    import BoilerImage from '$assets/boiler.jpg.avif';
    let plumbingModal = $state(false);
    let boilersModal = $state(false);
    let smartthermosModal = $state(false);
    let ashpModal = $state(false);
</script>

<section>
	<div class="container mx-auto mb-5 mt-5 lg:mt-15 lg:mb-15 flex flex-col p-2 lg:p-6 lg:flex-row">
    <div class="grid grid-cols-1 lg:grid-cols-2 lg:grid-rows-2 w-full gap-10">
        <div class="aspect-square" style="background-image: url({PlumbingImage}); background-position: 50%;">
           <div class="backdrop-brightness-25 w-full h-full text-white flex flex-col items-center justify-center space-y-20 p-10 text-center">
            <h2 class="text-6xl font-bold">Plumbing</h2>
            <button class="px-4 py-4 w-fit bg-amber-300 text-2xl text-black hover:cursor-pointer" onclick={() => plumbingModal = true}>Explore</button>
           </div> 
        </div>
        <div class="aspect-square" style="background-image: url({BoilerImage}); background-position: 90% 5%;">
            <div class="backdrop-brightness-25 w-full h-full text-white flex flex-col items-center justify-center space-y-20 p-10 text-center">
             <h2 class="text-6xl font-bold">Boilers and Heating Systems</h2>
             <button class="px-4 py-4 w-fit bg-amber-300 text-2xl text-black hover:cursor-pointer" onclick={() => boilersModal = true}>Explore</button>
            </div> 
         </div>
         <div class="aspect-square" style="background-image: url({SmartThermoImage}); background-position: 20% 35%;">
            <div class="backdrop-brightness-25 w-full h-full text-white flex flex-col items-center justify-center space-y-20 p-10 text-center">
             <h2 class="text-6xl font-bold">Smart Home Thermostats</h2>
             <button class="px-4 py-4 w-fit bg-amber-300 text-2xl text-black hover:cursor-pointer" onclick={() => smartthermosModal = true}>Explore</button>
            </div> 
         </div>
         <div class="aspect-square" style="background-image: url({ASHPImage})">
            <div class="backdrop-brightness-25 w-full h-full text-white flex flex-col items-center justify-center space-y-20 p-10 text-center">
             <h2 class="text-6xl font-bold">Air Source Heat Pumps</h2>
             <button class="px-4 py-4 w-fit bg-amber-300 text-2xl text-black hover:cursor-pointer" onclick={() => ashpModal = true}>Explore</button>
            </div> 
         </div> 
    </div>
</section>

<Modal bind:showModal={plumbingModal}>
    {#snippet header()}
        <h3 class="text-4xl">Plumbing Services</h3>
        <p class="text-xl">
            Our general plumbing services include a wide range of tasks and repairs related to the installation, maintenance, and repair of pipes, fixtures, and other plumbing systems. We also offer services such as conducting routine inspections, troubleshooting problems, and providing maintenance to help prevent future issues. 
        </p>
        <p class="text-xl">Common examples of the plumbing services we provide include:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1 text-xl">
        <li>Water leak repairs</li>
        <li>New pipe installation and repair</li>
        <li>Toilet repair and replacement</li>
        <li>Tap repair and replacement</li>
        <li>Hot water cylinder repair and installation</li>
        <li>Vented and unvented systems</li>
        <li>Water treatments</li>
        <li>Shower repair and installation</li>
        <li>Stopcock repair</li>
        <li>Radiator installation, repair or replacement</li>
        <li>Radiator valve fit or repair and replacement</li>
    </ul>
</Modal>
<Modal bind:showModal={boilersModal}>
    {#snippet header()}
        <h3 class="text-4xl">Boilers and Heating System - Service and Repairs</h3>
        <h4 class="text-3xl font-bold">Boiler Services</h4>
        <p class="text-xl">Having your boiler regularly serviced and maintained is essential to keep it running smoothly and avoiding any breakdowns. We recommend having your boiler serviced once a year to ensure it continues to run safely and efficiently.
            Our engineers are experienced in servicing all makes and models of gas boilers.
            Regular servicing not only extends the life of your boiler, but also helps in detecting any potential faults, saving you from costly repairs in the future.</p>
            <p class="text-xl font-bold">Our boiler services cost £70 + VAT</p>
        <h4 class="text-3xl font-bold">Boiler Repairs</h4>
        <p class="text-xl">
            When your boiler breaks down, our Gas Safe heating engineers can address a wide range of issues to restore warmth and comfort to your home and business. They can diagnose and repair problems such as faulty thermostats, leaking or frozen pipes, broken pilot lights, and malfunctioning pumps or valves. If the boiler isn’t producing heat or hot water, they will inspect components like the heat exchanger, ignition system, and pressure levels to identify the cause. In addition, they can handle blockages or buildup in the system, clean or replace filters, and ensure safety features like pressure relief valves are functioning correctly. Our engineer's expertise ensures a thorough and efficient repair, getting your boiler back in optimal working condition asap. 
        </p>
        <h4 class="text-3xl font-bold">Central Heating Installation & Maintenance</h4>
        <p class="text-xl">We provide full central heating system installations, including boilers, radiators, pipework, and controls. Additionally, we offer ongoing maintenance and repair services to keep your heating system in optimal condition.</p>
        <p class="text-xl font-bold">Installation Cost on Quotation</p> 
	{/snippet}
</Modal>
<Modal bind:showModal={smartthermosModal}>
    {#snippet header()}
        <h3 class="text-4xl">Smart Home Thermostats</h3>
        <p class="text-xl">
            A smart control for a boiler is a device that allows you to control and monitor your boiler remotely, typically using a smartphone app or a web interface. Some smart controls also have built-in learning algorithms that can optimise the performance of your boiler based on your usage patterns, helping to save energy and reduce your heating bills.
            Some common features of smart boiler controls include the ability to:
        </p>
        <ul class="text-xl list-disc p-5">
            <li>Set and adjust the temperature of your heating system</li>
            <li>Set schedules for when your heating should be on or off</li>
            <li>Monitor the status of your boiler and get alerts if there are any issues</li>
            <li>Monitor your energy usage and receive tips for saving energy</li>
            <li>Control your heating from anywhere using a smartphone app</li>
        </ul>
        <p class="text-xl">Smart controls can be particularly useful for people who are away from home for extended periods of time, as they can help to ensure that your heating is only turned on when it is needed. They can also be useful for people who have a large home or multiple heating zones, as they allow you to control and monitor all of your heating remotely.</p>
        <p class="text-xl font-bold">The types of Smart Thermostat we can supply and fit:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1 text-2xl">
        <li>Nest</li>
        <li>Hive</li>
        <li>Tado</li>
    </ul>
</Modal>
<Modal bind:showModal={ashpModal}>
    {#snippet header()}
        <h3 class="text-4xl">Heat Pumps - Service and Repair</h3>
        <p class="text-xl">
            A heat pump is a smart eco-friendly system which provides your home with sustainable, energy efficient warmth and hot water.
        </p>
        <p class="text-xl">
            Air source heat pumps draw heat from the surrounding air, the process works a bit like a refridgerator in reverse 
            and passes air through a heat exchanger to warm your home, keeping a comfortable ambient temperature.
        </p>
        <p class="text-xl font-bold">Benefits:</p>
	{/snippet}

    <ul class="list-disc ps-4 space-y-1 text-2xl">
        <li>Lower your energy bills</li>
        <li>Cut your carbon footprint</li>
        <li>Raise your property value</li>
        <li>Easier to maintain than combustion systems</li>
        <li>Often include warranties of up to 7 years</li>
    </ul>
    {#snippet button()}
    Contact Us For Site Surveys, Service and Repairs
    {/snippet}
</Modal>