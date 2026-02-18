<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let prepurchasesurveyFAQ: faq[] = [
        {question: "What is a pre-purchase heating and plumbing survey?", answer: "This is a detailed inspection of the boiler, heating system, and plumbing in a property you are considering buying, helping you understand its condition before committing."},
        {question: "Why should I have a survey before buying a property?", answer: "Heating and plumbing repairs can be costly. Our survey highlights potential issues, safety concerns, and future replacement costs so you can make an informed decision or renegotiate if needed."},
        {question: "What do you check during the survey?", answer: "We assess the boiler, radiators, pipework, hot water system, visible plumbing, and overall system condition, providing clear feedback and recommendations."},
        {question: "Will I receive a report?", answer: "Yes. You will receive a basic written summary of our findings and any recommended actions or likely future costs."},
        {question: "When should I book a pre-purchase survey?", answer: "Ideally once your offer has been accepted but before exchange of contracts, so you have a full understanding of what may be required before completion."},
        ]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="" faq={prepurchasesurveyFAQ} />
		</div>
	</div>
</section>