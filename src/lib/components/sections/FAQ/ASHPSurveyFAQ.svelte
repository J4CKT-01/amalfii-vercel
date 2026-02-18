<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let ashpsurveyFAQ: faq[] = [
        {question: "What is a heat pump suitability survey?", answer: "Our heat pump suitability survey is designed for homeowners who are considering an air source heat pump and want to know if their property is suitable. We assess your current heating system, insulation, radiators, and property layout to give clear, honest advice before any major decisions are made."},
        {question: "Why do I need a survey before installing a heat pump?", answer: "Heat pumps work differently to traditional boilers and must be correctly designed for the property. A professional survey ensures your home can achieve good comfort levels and efficiency and highlights any improvements that may be needed before installation."},
        {question: "What do you check during the survey? ", answer: "We assess insulation levels, radiator sizes, pipework, hot water systems, available outdoor space, and your current heating performance. This helps us understand whether a heat pump would work well in your home and what changes may be required."}, 
        {question: "Will you tell me honestly if a heat pump isn’t right for my home? ", answer: "Yes. Our approach is always honest and practical. If a heat pump is not currently the best option for your property, we will explain why and discuss alternative solutions or future improvements that could make it viable."}, 
        {question: "Which survey will I need?", answer: `We offer two levels of heat pump suitability survey, depending on how much detail you would like and where you are in your decision-making process. 
        Our basic suitability survey is ideal if you are at an early stage and would like honest, professional guidance on whether a heat pump could work in your home. We assess your current heating system, radiators, insulation and general property suitability, and provide clear verbal feedback and recommendations. This survey costs £120 +vat 
        Our in-depth suitability survey is designed for homeowners who are seriously considering a future heat pump installation. This more detailed assessment looks closely at system design considerations, radiator sizing, hot water provision and overall efficiency, helping you understand what would be required for a successful installation. This survey costs £295+vat and will come with a detailed report  
        If you are unsure which level is right for you, we are always happy to guide you towards the most appropriate survey for your home and plans.`}, 
        ]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="" faq={ashpsurveyFAQ} />
		</div>
	</div>
</section>