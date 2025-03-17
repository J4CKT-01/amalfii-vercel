<script lang="ts">
	import FleetImage from '$assets/fleet.png';
	import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-5 flex justify-between flex-col-reverse p-2 lg:p-6 lg:mt-15 lg:flex-row max-h-min">
		<div class="w-full flex flex-row justify-start" style="background-image: url({FleetImage}); background-size: cover;">
			<div class="space-y-5 lg:space-y-15 p-6 text-left w-full lg:p-10 lg:w-1/2 backdrop-brightness-25 text-white">
				<Header>About us</Header>
				<p class=" text-2xl">
					We are a small local company, established in 2018, consisting of heating engineers and plumbers, air conditioning engineers and heat 
					pump installers who work the M5 corridor, from Worcestershire and Gloucestershire down to south Bristol.
					Our friendly team is highly experienced, efficient and affordable. We are Gas Safe, F-Gas and Heat Pump certified
					 for your peace of mind. If you need plumbing or heating solutions, we're the team to trust. Great customer service 
					 is of the utmost importance to us and our office team will take your calls and manage your visits so your experience with 
					 us is easy and stress free!
				</p>
			</div>
		</div>
	</div>
</section>
