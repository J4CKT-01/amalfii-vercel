<script lang="ts">
	import KarenImage from '$assets/karen.jpg';
	import SimonImage from '$assets/simon.jpg';
	import HannahImage from '$assets/hannah.jpg';
	import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-5 mb-5 p-2 lg:mt-15 lg:mb-15 lg:p-6">
		<div class="mb-15 w-full text-center"><Header>Meet The Team</Header></div>
		<div class="grid grid-cols-1 gap-20 lg:grid-cols-3">
			<div class="flex flex-col space-y-5 items-center text-center p-6 shadow-md">
				<img class="size-48 rounded-full object-cover" src={KarenImage} alt="" />
				<div>
				    <h4 class="text-2xl font-bold">Karen</h4>
    				<h5 class="text-gray-500">Office Manager</h5>
				</div>
				<p>
					As the office manager at Amalfii Heating, Karen is the first point of contact for customers,
                     ensuring everything rusn smoothly behind the scenes. She handles job bookings, schedule appointments, 
                     and make sure the engineers have all the details they need to get the job done efficiently. Whether you need 
                     a routine service, an emergency repair, or just some advice, Karen is here to help make the process as easy and 
                     stress-free as possible!
				</p>
			</div>
			<div class="flex flex-col space-y-5 items-center text-center p-6 shadow-md">
				<img class="size-48 rounded-full object-cover" src={SimonImage} alt="" />
				<div>
				    <h4 class="text-2xl font-bold">Simon</h4>
    				<h5 class="text-gray-500">Lead Engineer</h5>
				</div>
				<p>
					Simon is Amalfii Heating's lead engineer. Simon trained with one of the leading energy suppliers 25 years ago and has been working as a gas heating engineer and plumber ever since. Simon is Gas Safe registered, highly qualified and experienced and prides himself on providing fair, efficient and reliable services to our customers. 

Recently Simon has acquired qualifications in providing service and maintenance of air source heat pumps, keeping our company moving forward into a greener era.  
				</p>
			</div>
			<div class="flex flex-col space-y-5 items-center text-center p-6 shadow-md">
				<img class="size-48 rounded-full object-cover" src={HannahImage} alt="" />
				<div>
				    <h4 class="text-2xl font-bold">Hannah</h4>
    				<h5 class="text-gray-500">Assistant Receptionist</h5>
				</div>
				<p>
					You may speak to Hannah on occasions! Hannah helps Karen out in the office, taking calls, and scheduling work in and, after completion of her digital marketing course, will be coming on board with us to showcase her social media skills!  
				</p>
			</div>
		</div>
	</div>
</section>
