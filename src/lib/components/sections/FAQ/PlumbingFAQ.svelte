<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let plumbingFAQ: faq[] = [
        {question: "What plumbing services do you offer?", answer: "We carry out a full range of domestic plumbing services including leaks, tap and toilet repairs, radiator installations and repairs, hot water issues, and general plumbing maintenance. We focus on reliable, long-term solutions rather than temporary fixes."},
        {question: "Do you take on small plumbing jobs as well as larger work?", answer: "Yes. We are happy to undertake smaller plumbing repairs such as leaks, faulty taps, and radiator bleeding, as well as larger planned works and heating system replacement or improvements."},
        {question: "How quickly can you attend a plumbing problem?", answer: "We aim to attend urgent plumbing and heating issues as quickly as possible. All repair visits are booked as diagnostic so we can properly assess the problem and provide the best solution."},
        {question: "Do you provide quotes before carrying out work?", answer: "Yes. Any work beyond the initial diagnostic visit will always be clearly explained and quoted before proceeding, so you remain fully in control of costs."},
        {question: "Why choose Amalfii Heating for plumbing work?", answer: "We are an experienced, professional heating and plumbing company known for honest advice, quality workmanship, and a reliable service. Our goal is to keep your home safe, comfortable, and running efficiently."},
	]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="" faq={plumbingFAQ} />
		</div>
	</div>
</section>