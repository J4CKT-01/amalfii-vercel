<script lang="ts">
	import { Header } from '$lib';
	import Thermostat from '$assets/thermostat.png';
</script>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-6 lg:flex-row max-h-min">
		<div class="hidden lg:flex w-full items-center justify-center lg:w-1/3">
				<img
					class="h-full aspect-square w-full object-cover"
					src={Thermostat}
					alt=""
				/>
		</div>
		<div class="mb-15 w-full space-y-10 p-10 text-center lg:mb-0 lg:w-2/3 lg:text-left">
			<Header>Smart Home Thermostats</Header>
			<p class=" text-3xl">
				A smart control for a boiler is a device that allows you to control and monitor your boiler
				remotely, typically using a smartphone app or a web interface. Some smart controls also have
				built-in learning algorithms that can optimise the performance of your boiler based on your
				usage patterns, helping to save energy and reduce your heating bills.
			</p>
            <div class="flex flex-row justify-evenly lg:space-x-40">
                <div class="flex flex-col items-center xl:items-start">
                    <i class="fa-sharp-duotone fa-regular fa-leaf text-5xl mb-5"></i>
                    <p class="text-4xl font-bold">Nest</p>
                </div>
                <div class="flex flex-col items-center xl:items-start">
                    <i class="fa-sharp-duotone fa-regular fa-hexagon text-5xl mb-5"></i>
                    <p class="text-4xl font-bold">Hive</p>
                </div>
                <div class="flex flex-col items-center xl:items-start">
                    <i class="fa-sharp-duotone fa-regular fa-circle-t text-5xl mb-5"></i>
                    <p class="text-4xl font-bold">Tado</p>
                </div>
            </div>	
		</div>
	</div>
</section>
