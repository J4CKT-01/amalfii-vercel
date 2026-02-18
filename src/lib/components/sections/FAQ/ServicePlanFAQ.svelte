<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let serviceplanFAQ: faq[] = [
        {question: "What are the benefits of joining a service plan?", answer: "Our service plans help you spread the cost of essential annual servicing while keeping your heating system safe, efficient and reliable. Members also benefit from priority booking and discounted labour on repairs, giving added peace of mind throughout the year."},
        {question: "What is included in an Amalfii Heating service plan?", answer: "Each plan includes your annual boiler service and ongoing support to help keep your heating system running smoothly. You’ll also receive priority response for breakdowns and a discount on repair labour should any issues arise."},
        {question: "Do I need to have my boiler serviced before joining a plan?", answer: "In most cases, yes. We recommend that your boiler is serviced or assessed by us before joining to ensure it is safe and in good working order. This allows us to maintain your system correctly in line with manufacturer recommendations going forward."},
        {question: "Can I join a plan if we didn’t install my boiler?", answer: "Absolutely. Many of our customers join our service plans even if their boiler or heating system was installed by another company. We simply carry out an initial service or assessment before the plan begins."},
        {question: "Who are your service plans suitable for?", answer: "Our plans are suitable for homeowners and landlords who want a simple, affordable way to maintain their heating system and avoid unexpected repair costs. They are ideal for anyone who values regular servicing, priority support and long-term reliability."},
        ]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="" faq={serviceplanFAQ} />
		</div>
	</div>
</section>