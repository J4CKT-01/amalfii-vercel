<script lang="ts">
	import FleetImage from '$assets/fleet.png';
	import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-6 lg:flex-row">
		<div class="flex w-full items-center justify-center lg:w-1/2 lg:pr-25">
			<div>
				<img
					class=" h-100 w-full rounded-2xl object-cover object-right lg:mb-15"
					src={FleetImage}
					alt=""
				/>
			</div>
		</div>
		<div class="mb-15 w-full space-y-10 lg:space-y-25 text-center lg:mb-0 lg:w-1/2 lg:text-left">
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
