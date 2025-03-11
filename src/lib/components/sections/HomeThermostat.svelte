<script lang="ts">
	import { Header } from '$lib';
	import Thermostat from '$assets/thermostat.png';
</script>

<section>
	<div class="container mx-auto mt-15 mb-15 flex flex-col p-6 shadow-2xl lg:flex-row">
		<div class="hidden xl:w-1/2 lg:pr-25 lg:block">
			<img class="h-175 w-full object-cover" src={Thermostat} alt="" />
		</div>
		<div class="mb-15 w-full space-y-10 lg:mb-0 xl:w-1/2 lg:space-y-25 text-center xl:text-left">
			<Header>Smart Home Thermostats</Header>
			<p class=" text-3xl">
				A smart control for a boiler is a device that allows you to control and monitor your boiler
				remotely, typically using a smartphone app or a web interface. Some smart controls also have
				built-in learning algorithms that can optimise the performance of your boiler based on your
				usage patterns, helping to save energy and reduce your heating bills.
			</p>
            <div class="grid grid-cols-3">
                <div class="flex flex-col items-center xl:items-start">
                    <i class="fa-sharp-duotone fa-regular fa-leaf text-7xl mb-5"></i>
                    <p class="text-4xl font-bold">Nest</p>
                </div>
                <div class="flex flex-col items-center xl:items-start">
                    <i class="fa-sharp-duotone fa-regular fa-hexagon text-7xl mb-5"></i>
                    <p class="text-4xl font-bold">Hive</p>
                </div>
                <div class="flex flex-col items-center xl:items-start">
                    <i class="fa-sharp-duotone fa-regular fa-circle-t text-7xl mb-5"></i>
                    <p class="text-4xl font-bold">Tado</p>
                </div>
            </div>
		</div>
	</div>
</section>
