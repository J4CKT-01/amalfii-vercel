<script lang="ts">
	import { Header, FAQ } from "$lib";
    import type { faq } from '../../FAQ.svelte';

    let smarthomeFAQ: faq[] = [
        {question: "What are the benefits of smart heating controls?", answer: "Smart thermostats and smart radiator valves give you greater control over your heating, allowing you to adjust temperatures remotely, create heating schedules, and heat individual rooms more efficiently."},
        {question: "Can smart controls help reduce energy bills?", answer: "Yes. By heating only the rooms you need and controlling your system more precisely, many homeowners find smart controls help improve efficiency and reduce energy usage."},
        {question: "Can you supply and install smart thermostats and smart radiator valves?", answer: "We can advise on, supply, and install a range of trusted smart heating controls. We also set up the system fully and show you how to use it so you feel confident managing your heating."},
        {question: "Will smart controls work with my existing boiler?", answer: "Most modern boilers are compatible with smart thermostats, but we will always check your current system and recommend the most suitable controls for your home."},
        {question: "Do I need Wi-Fi for smart heating controls?", answer: "Yes, a stable internet connection is required for full smart functionality such as app control and remote access. We will ensure everything is connected and working before we leave. Once installed and working correctly, any connection issues should be taken up with the manufacturer although we will endeavor to help first."},
	]
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<FAQ title="" faq={smarthomeFAQ} />
		</div>
	</div>
</section>