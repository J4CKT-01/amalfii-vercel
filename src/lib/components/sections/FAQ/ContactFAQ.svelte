<script lang="ts">
	import { Accordion, Header, FAQ } from '$lib';
	import { createRawSnippet } from 'svelte';
	import type { faq } from '../../FAQ.svelte';

	let generalFAQ: faq[] = [
		{question: "What services do you offer?", answer: "We provide a full range of plumbing, heating and air source heat pump services, including boiler installation, service and repairs, central heating servicing, radiator installation, leak detection, smart thermostats and much more!"},
		{question: "Are you a Gas Safe registered company?", answer: "Yes, we are fully Gas Safe registered and qualified to work on gas appliances safely. You can verify our credentials on the Gas Safe Register  www.gassaferegister.co.uk"},
		{question: "Do you offer 24hr emergency callouts?", answer: "No, we do not offer 24/7 emergency callouts, however, we will come out to you as soon as we possibly can. If you have an uncontainable leak, turn off the water at the stopcock"},
		{question: "What if I smell gas?", answer: "", children: createRawSnippet(() => ({
		render() {
			return `
						<ol class="list-decimal pl-10">
					<li><span class="font-bold">Do not ignore it.</span> Smelling gas can be sign of a leak and can be dangerous.</li>
					<li>Don't use electrical devices that could cause a spark and <span class="font-bold">DON'T</span> use matches or lighters.</li>
					<li><span class="font-bold">CALL FOR HELP</span> from a safe location. Call the National Gas Emergency Service immediately on 0800 111 999 (24hrs free phone).</li>
					<li>Open windows and doors.</li>
					<li>Evacuate the area.</li>
				</ol>
						`
				}
		}))},
		{question: "What areas do you cover?", answer: "We serve Worcestershire, Gloucestershire and the M5 corridor down to Bristol. Contact us to check if we operate in your area."},
		{question: "Do you offer free quotes?", answer: "Yes! We provide free, no-obligation quotes for all our services. Simply contact us to arrange an assessment."},
		{question: "I am a landlord, why do I need gas certificates and carbon monoxide detectors?", 
		answer: `As a landlord you are responsible for the safety of your tenants, the gas safety
                regulations specifically deal with the duties of landlords to ensure that gas appliances,
				fittings and flues are safe for tenants to use. Safety checks and servicing are a legal
				requirement. They ensure that the appliances are operating safely and are not producing
				lethal carbon monoxide. All gas fittings, pipe work, flues and ventilation must be inspected
				and tested. This work must be done by a GAS SAFE registered installer who will service the
				appliances and fill our the landlords safety certificate. We also recommend installing a 
				carbon monoxide detector in any room containing a gas appliance. There are various types of 
				carbon monoxide detectors that give visual or auditory indication of carbon monoxide buildup. 
				Contact us to find out more.`}
	]

	let pricingFAQ: faq[] = [
		{question: "How much do your services cost?", answer: "Prices vary depending on the service required. We offer competitive rates and free quotes, so contact us for an estimate."},
		{question: "Do you offer boiler or air pump maintenance plans?", answer: "Yes we offer monthly payment service plans for boilers, boiler and gas fire, Landlord Gas Safety Inspections and Air Source Heat pump servicing. You will not pay any more for your service but the plan will allow you to spread the cost over 12 months and have the benefit of 15% discount on any labour charge should your boiler or heat pump need repairs."},
		{question: "Do you offer financing options for new boilers?", answer: "No, not at this present time"},
		{question: "What payment methods do you accept?", answer: "We accept cash, bank transfers and most major debit/credit cards. As well as monthly direct debits for all our servicing plans."},
		{question: "Are your services guaranteed?", answer: "Yes, all our work is fully guaranteed for your peace of mind."},
		{question: "Do you offer landlord gas safety certificates?", answer: "Yes, we provide Gas Safety Certificates (CP12) for landlords and letting agents."},
	]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="General" faq={generalFAQ} />
			<FAQ title="Pricing and Payments" faq={pricingFAQ} />
		</div>
	</div>
</section>
