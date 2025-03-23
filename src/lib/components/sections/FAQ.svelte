<script>
	import { Accordion, Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-5 flex flex-col items-center p-2 lg:p-6">
		<div class="my-5 lg:mb-10">
			<Header>Frequently Asked Questions</Header>
		</div>
		<div class="w-full space-y-5">
			<Header>General</Header>
			<Accordion
				title="What services do you offer?"
				content="We provide a full range of plumbing, heating and air source heat pump services, including boiler installation, service and repairs, central heating servicing, radiator installation, leak detection, smart thermostats and much more! "
			/>
			<Accordion
				title="Are you a Gas Safe registered company?"
				content="Yes, we are fully Gas Safe registered and qualified to work on gas appliances safely. You can verify our credentials on the Gas Safe Register  www.gassaferegister.co.uk "
			/>
			<Accordion
				title="Do you offer 24hr emergency callouts?"
				content="No, we do not offer 24/7 emergency callouts, however, we will come out to you as soon as we possibly can. If you have an uncontainable leak, turn off the water at the stopcock "
			/>
			<Accordion
				title="What if I smell gas?"
				content=""
			>
			{#snippet list()}			
				<ol class="list-decimal pl-10">
					<li><span class="font-bold">Do not ignore it.</span> Smelling gas can be sign of a leak and can be dangerous.</li>
					<li>Don't use electrical devices that could cause a spark and <span class="font-bold">DON'T</span> use matches or lighters.</li>
					<li><span class="font-bold">CALL FOR HELP</span> from a safe location. Call the National Gas Emergency Service immediately on 0800 111 999 (24hrs free phone).</li>
					<li>Open windows and doors.</li>
					<li>Evacuate the area.</li>
				</ol>
			{/snippet}
			</Accordion>
			<Accordion
				title="What areas do you cover?"
				content="We serve Worcestershire, Gloucestershire and the M5 corridor down to Bristol. Contact us to check if we operate in your area. "
			/>
			<Accordion
				title="Do you offer free quotes?"
				content="Yes! We provide free, no-obligation quotes for all our services. Simply contact us to arrange an assessment."
			/>
			<Accordion
				title="I am a landlord, why do I need gas certificates and carbon monoxide detectors?"
				content="As a landlord you are responsible for the safety of your tenants, the gas safety
                 regulations specifically deal with the duties of landlords to ensure that gas appliances,
                  fittings and flues are safe for tenants to use. Safety checks and servicing are a legal
                   requirement. They ensure that the appliances are operating safely and are not producing
                    lethal carbon monoxide. All gas fittings, pipe work, flues and ventilation must be inspected
                     and tested. This work must be done by a GAS SAFE registered installer who will service the
                      appliances and fill our the landlords safety certificate. We also recommend installing a 
                      carbon monoxide detector in any room containing a gas appliance. There are various types of 
                      carbon monoxide detectors that give visual or auditory indication of carbon monoxide buildup. 
                      Contact us to find out more."
			/>
			<Header>Pricing and Payments</Header>
			<Accordion
				title="How much do your services cost?"
				content="Prices vary depending on the service required. We offer competitive rates and free quotes, so contact us for an estimate."
			/>
			<Accordion
				title="Do you offer boiler or air pump maintenance plans?"
				content="Yes we offer monthly payment service plans for boilers, boiler and gas fire, Landlord Gas Safety Inspections and Air Source Heat pump servicing. You will not pay any more for your service but the plan will allow you to spread the cost over 12 months and have the benefit of 15% discount on any labour charge should your boiler or heat pump need repairs. "
			/>
			<Accordion
				title="Do you offer financing options for new boilers? "
				content="No, not at this present time"
			/>
			<Accordion
				title="What payment methods do you accept?"
				content="We accept cash, bank transfers and most major debit/credit cards. As well as monthly direct debits for all our servicing plans."
			/>
			<Accordion
				title="Are your services guaranteed?"
				content="Yes, all our work is fully guaranteed for your peace of mind."
			/>
			<Accordion
				title="Do you offer landlord gas safety certificates?"
				content="Yes, we provide Gas Safety Certificates (CP12) for landlords and letting agents."
			/>
			<Header>Plumbing</Header>
			<Accordion
				title="Why is my tap dripping?"
				content="A dripping tap is usually caused by a worn washer or faulty valve. 
            We can repair or replace it quickly"
			/>
			<Accordion
				title="What should I do if I have a burst pipe?"
				content="Turn of your main water supply immediately and contact us for emergency 
            assistance."
			/>
			<Accordion
				title="My toilet won't flush - can you help?"
				content="Yes! Common causes include a faulty flush mechanism or a blocked pipe. 
            We can diagnose and fix the issue promptly."
			/>
			<Accordion
				title="What should I do if my water pressure is low?"
				content="Low water pressure could be due to a blockage, a leak, or an issue 
            with the mains supply. Contact us to investigate and resolve the problem."
			/>
			<Header>Boilers and Heating</Header>
			<Accordion
				title="How often should I service my boiler?"
				content="We recommend servicing your boiler once a year to ensure efficiency, safety, and to prevent breakdowns."
			/>
			<Accordion
				title="What boiler brands do you install and repair?"
				content="We install, repair and service leading brands such as Worcester Bosch, Vaillant, Ideal, Baxi and many more."
			/>
			<Accordion
				title="My boiler is making strange noises - what should I do?"
				content="Noisy boilers can be caused by air in the system, low pressure, or limescale buildup. Contact us for an inspection before it leads to bigger issues."
			/>
			<Accordion
				title="How do I know if I need a new boiler?"
				content="If your boiler is over 10-15 years old, frequently breaking down, or inefficient, it may be time for an upgrade. We can advise you on the best options."
			/>
			<Accordion
				title="Do you offer power flushes?"
				content="No, unfortunately we do not offer this as a service but we will put you in contact with engineers who can."
			/>
            <Accordion
				title="Do you offer heat pump servicing?"
				content="Yes, we can service air source heat pumps."
			/>
            <Accordion
				title="How often should my air source heat pump be serviced?"
				content="We recommend that your system is serviced annually."
			/> 
		</div>
	</div>
</section>
