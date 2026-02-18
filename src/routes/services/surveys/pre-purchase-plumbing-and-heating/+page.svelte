<script lang="ts">
	import { Header, PrePurchaseSurveyFAQ, Title } from "$lib";
    import Fleet from "$assets/fleet.png";

    let services = [
        "Boiler age, condition and general safety",
        "Heating system type and overall condition",
        "Radiators. controls and visible pipework",
        "Hot water systems",
        "General plumbing installation",
        "Any visible concerns or potential future issues"
    ]

</script>

<svelte:head>
    <title>Pre-Purchase Plumbing and Heating Surveys</title>
</svelte:head>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Pre-Purchase Plumbing and Heating Surveys</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Overview</Header>
                    <p class="text-xl">Buying a property is a big commitment, and the condition of the heating and plumbing system can have a significant impact on future costs.
                        At Amalfii Heating we offer pre-purchase plumbing and heating surveys to give you a clear, honest overview of the system before you proceed. This can be particularly helpful where
                         a property has an older boiler or heating system, or where you simply want reassurance and realistic guidance before exchange. These surveys are often requested following a homebuyer survey where heating or plumbing concerns have been highlighted.</p>
                </div>
                <div class="space-y-5 flex">
                    <img class="" src={Fleet} alt="">
                </div>
            </div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>What we look at:</Header></div>
    <div class="grid xl:grid-cols-3 gap-5 p-6">
        {#each services as service}
        <div class="flex items-top text-2xl p-6">
            <i class="fa-sharp-duotone fa-regular fa-circle-check me-5 mt-1"></i>
            <p>{service}</p>
        </div>
        {/each}
    </div>
    <div>
        <p class="text-xl p-6 font-semibold">We will talk through our findings clearly and can provide a short written summary if required, along with realistic guidance on likely future repair or replacement costs.</p>
    </div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10 items-center">
                <div class="p-6 space-y-5">
                    <Header>Why consider a separate heating & plumbing survey?</Header>
                    <p class="text-xl">Standard homebuyer surveys don’t usually assess heating and plumbing systems in detail.
                    A dedicated inspection can help you understand:</p>
                    <ul class="text-xl space-y-5 list-disc ms-5">
                        <li>the general condition and reliability of the system</li>
                        <li>whether upgrades may be needed in the future</li>
                        <li>likely maintenance or replacement costs</li>
                        <li>any immediate concerns that may need attention</li>
                    </ul>
                    <p class="text-xl">This allows you to make informed decisions and avoid unexpected surprises after moving in.</p>
                </div>
                <div class="p-6 space-y-5 bg-amber-300 h-max">
                    <div class="**:decoration-black"><Header>A straightforward, honest approach</Header></div>
                    <p class="text-xl">
                        Our surveys provide a clear, professional opinion on the visible condition and suitability of your heating and plumbing system at the time of inspection, based on what can be seen and our experience of installing and maintaining heating systems. They are non-invasive visual inspections, with no parts dismantled. This is not a sales visit — we do not use pressure or sales tactics. We will always be honest and realistic in our advice, explaining any concerns in plain language so you can make an informed decision about how you wish to proceed, whether that’s simply gaining clarity or exploring options.
                    </p>
                </div>
            </div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>Pricing</Header></div>
    <div class="grid xl:grid-cols-3 gap-5 p-6">
        <div class="flex flex-col justify-center items-center text-2xl p-6 space-y-10 border">
            <i class="fa-sharp-duotone fa-regular fa-house text-6xl"></i>
            <div class="h-15"><p class="text-2xl">Standard Local Property</p></div>
            <p class="text-3xl font-semibold">£250</p>
        </div>
        <div class="flex flex-col justify-center items-center text-2xl p-6 space-y-10 border">
            <i class="fa-sharp-duotone fa-regular fa-house-turret text-6xl"></i>
            <div class="h-15"><p class="text-2xl">Large Property</p></div>
            <p class="text-3xl font-semibold">£300</p>
        </div>
        <div class="flex flex-col justify-center items-center text-2xl p-6 space-y-10 border text-center">
            <i class="fa-sharp-duotone fa-regular fa-house-chimney-crack text-6xl"></i>
            <div class="h-15"><p class="text-2xl">Properties Needing Extensive Renovation</p></div>
            <p class="text-3xl font-semibold">£400</p>
        </div>
    </div>
</section>

<PrePurchaseSurveyFAQ />