<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let ashpFAQ: faq[] = [
        {question: "What is an air source heat pump?", answer: "An air source heat pump is an energy-efficient heating system that extracts heat from the outside air to provide heating and hot water for your home."},
        {question: "Are heat pumps suitable for all homes?", answer: "Not every property is immediately suitable. We carry out detailed surveys to assess insulation, radiators, pipework, and available space to determine whether a heat pump will work efficiently for you."},
        {question: "Are air source heat pumps energy efficient?", answer: "When correctly designed and installed, heat pumps can be highly efficient and provide comfortable, steady heating with lower carbon emissions compared to traditional systems."},
        {question: "Can a heat pump replace my gas boiler?", answer: "In many cases yes, but the system must be properly designed for your property. We provide honest advice on whether a full or partial transition would work best."},
        {question: "Do you service and maintain heat pumps?", answer: "Yes. We provide servicing, maintenance, and performance checks to keep heat pumps running efficiently and reliably."},
	]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="" faq={ashpFAQ} />
		</div>
	</div>
</section>