<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let boilerFAQ: faq[] = [
        {question: "How often should I service my boiler?", answer: "We recommend servicing your boiler once a year to ensure efficiency, safety, and to prevent breakdowns."},
        {question: "What boiler brands do you install and repair?", answer: "We install, repair and service leading brands such as Worcester Bosch, Vaillant, Ideal, Baxi and many more."},
        {question: "My boiler is making strange noises - what should I do?", answer: "Noisy boilers can be caused by air in the system, low pressure, or limescale buildup. Contact us for an inspection before it leads to bigger issues."},
        {question: "How do I know if I need a new boiler?", answer: "If your boiler is over 10-15 years old, frequently breaking down, or inefficient, it may be time for an upgrade. We can advise you on the best options."},
        {question: "Do you offer power flushes?", answer: "No, unfortunately we do not offer this as a service but we will put you in contact with engineers who can."},
	]
    let boilerrepairFAQ: faq[] = [
		{question: "Do you charge a call-out fee?", answer: "All repair visits are booked as a diagnostic visit, which covers attendance, fault-finding, safety checks and up to the first hour of labour."},
		{question: "What if the repair takes longer than one hour?", answer: "Any additional labour will be discussed with you and charged in 30-minute increments."},
		{question: "What if parts are needed?", answer: "If parts are required, we will explain this on the day and provide a clear price before ordering or carrying out further work."},
		{question: "Will I be charged if the issue can't be fixed on the first visit?", answer: "The diagnostic visit covers time spent assessing and identifying the fault. If further work is required, this will be clearly quoted before proceeding."},
		{question: "What if the problem returns?", answer: "We stand by our workmanship. If the same repair fails due to our work, we will return free of charge. If a separate fault develops, a further diagnostic visit may be required."},
		{question: "Do you offer fixed-price repairs?", answer: "Some repairs can be priced in advance. Where this isn't possible, we will always explain costs clearly before any work is carried out."},
        {question: "Are diagnostic visits refundable if I choose not to proceed?", answer: "Diagnostic visits cover the engineer’s time, assessment and safety checks and are therefore non-refundable."},
	]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="Boiler Servicing" faq={boilerFAQ} />
            <FAQ title="Boiler Repairs" faq={boilerrepairFAQ} />
		</div>
	</div>
</section>

