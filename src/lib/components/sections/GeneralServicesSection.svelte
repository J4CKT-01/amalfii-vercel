<script lang="ts">
	import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-15 flex flex-col p-6 lg:flex-row">
        <div class="flex flex-col justify-center mb-15 w-full space-y-10 lg:space-y-25 text-center lg:mb-0 lg:w-1/2 lg:text-left">
            <Header>General services we provide</Header>
            <p class=" text-3xl">
                In addition to service plans, Amalfii Heating can help with a variety of plumbing and 
                heating issues. We provide repairs, installations and one off services to....
            </p>
        </div>
        <div class="w-full grid grid-rows-2 grid-cols-2 gap-20 lg:w-1/2">
            <div class="flex flex-col justify-evenly items-center space-y-5 h-40">
                <i class="fa-sharp-duotone fa-regular fa-pipe-valve text-5xl mt-6"></i>
                <p class="text-4xl">Plumbing</p>
            </div>
            <div class="flex flex-col justify-evenly items-center h-40">
                <i class="fa-sharp-duotone fa-regular fa-droplet-degree text-5xl mt-6"></i>
                <p class="text-4xl">Boilers</p>
            </div>
            <div class="flex flex-col justify-evenly items-center h-40">
                <i class="fa-sharp-duotone fa-regular fa-oven text-5xl mt-6"></i>
                <p class="text-4xl text-center">Gas Appliances</p>
            </div>
            <div class="flex flex-col justify-evenly items-center h-40">
                <i class="fa-sharp-duotone fa-regular fa-air-conditioner text-5xl mt-6"></i>
                <p class="text-4xl">ASHP</p>
            </div>
        </div>
	</div>
</section>
