<script lang="ts">
	import FleetImage from '$assets/fleet.png';
	import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-5 flex justify-between flex-col-reverse p-2 lg:p-6 lg:mt-15 lg:flex-row max-h-min">
		<div class="flex w-full items-center justify-center lg:w-2/5">
				<img
					class="h-full w-full object-cover rounded-3xl"
					src={FleetImage}
					alt=""
				/>
		</div>
		<div class="mb-5 w-full space-y-10 lg:space-y-25 lg:mb-0 lg:w-1/2 text-left lg:p-10">
			<Header>About us</Header>
			<p class=" text-3xl">
				Amalfii Heating is a family run company, built with 25 years of experience covering all
				areas of home heating, plumbing and boilers. We have experience working in a wide range of
				buildings, from new builds to victorian-era houses! Whether you are looking purely for a
				service plan for your home, a quick repair, or need a complete refit of your infrastructure,
				Amalfii Heating has you covered!
			</p>
		</div>
	</div>
</section>
