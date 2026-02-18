<script lang="ts">
	import { Header, ASHPSurveyFAQ, Title } from "$lib";
    import Fleet from "$assets/fleet.png";

    let services = [
        "Current boiler and heating system",
        "Radiator sizes and pipework",
        "Hot water cylinder and available space",
        "Insulation levels and general property suitability",
        "Possible outdoor unit location",
        "Practical installation considerations",
        "General running and efficiency expectations"
    ]

</script>

<svelte:head>
    <title>Air Source Heat Pump Suitability Surveys</title>
</svelte:head>

<section>
	<div class="container mx-auto mt-15 flex flex-col-reverse p-2 lg:p-6 lg:flex-row">
		<div class="w-full space-y-10 lg:space-y-15 lg:text-center lg:mb-0">
			<Title>Air Source Heat Pump Suitability Surveys</Title>           
		</div>
	</div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Overview</Header>
                    <p class="text-xl">With more households considering low-carbon heating, many customers are asking whether an air source heat pump would work in their home.
                    At Amalfii Heating we offer air source heat pump suitability surveys to provide clear, honest and practical advice before any decisions are made.
                    This service is ideal if you are exploring heat pumps but want an experienced, independent view of whether your property is likely to be suitable.
                    </p>
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
            <div class="grid xl:grid-cols-2 gap-10">
                <div class="p-6 space-y-5">
                    <Header>Important information</Header>
                    <p class="text-xl font-semibold">This visit is a non-invasive visual suitability assessment only.
            No system design or heat loss calculations are carried out and no parts are dismantled. If more advanced surveys are required please contact us.
            Where appropriate, we may recommend that a full design assessment is undertaken by an MCS-accredited installer should you wish to proceed further.
</p>
                </div>
                <div class="p-6 space-y-5 bg-amber-300 h-max">
                    <div class="**:decoration-black"><Header>A straightforward, honest approach</Header></div>
                    <p class="text-xl">
                        Our surveys provide a clear, professional opinion on the visible condition and suitability of your heating and plumbing system at the time of inspection, based on what can be seen and our experience of installing and maintaining heating systems. They are non-invasive visual inspections, with no parts dismantled. This is not a sales visit — we do not use pressure or sales tactics. We will always be honest and realistic in our advice, explaining any concerns in plain language so you can make an informed decision about how you wish to proceed, whether that’s simply gaining clarity or exploring options.
                    </p>
                </div>
            </div>
            <div>
</section>

<section class="container mx-auto mt-5 p-2 lg:p-6 space-y-15">
    <div class="w-full xl:ps-6 xl:justify-start justify-center flex"><Header>Pricing</Header></div>
    <div class="grid xl:grid-cols-3 gap-5 p-6">
        <div class="flex flex-col justify-center items-center text-2xl p-6 space-y-10 border">
            <i class="fa-sharp-duotone fa-regular fa-house text-6xl"></i>
            <p class="text-2xl">Standard Local Property</p>
            <p class="text-3xl font-semibold">£150</p>
        </div>
    </div>
</section>


<ASHPSurveyFAQ />