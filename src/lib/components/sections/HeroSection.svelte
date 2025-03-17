<script lang="ts">
	import { goto } from '$app/navigation';
    import HeroImage from '$assets/hero.jpg.avif';
    import GasSafe from '$assets/gassafe.png';
</script>


<section>
    <div class="container grid auto-rows-fr lg:grid-cols-2 mx-auto items-center p-2 lg:p-6 mt-5 lg:mt-15">
        <div class="flex flex-col justify-center h-full space-y-15 text-center lg:text-left">
        <h1 class="text-8xl font-bold">Amal<span class="text-amber-300">fii</span> Heating</h1>
        <h2 class="text-4xl">Experts in home heating solutions</h2>
            <div class="flex flex-row lg:space-x-15 lg:flex-row justify-evenly lg:justify-start">
                <a href="/services">
                    <div class="flex flex-col items-center space-y-2">
                        <i class="fa-sharp-duotone fa-regular fa-sign-posts-wrench text-5xl"></i>
                        <h3 class="text-2xl">Installations</h3>
                    </div>
                </a>
                <a href="/services">
                    <div class="flex flex-col items-center space-y-2">
                        <i class="fa-sharp-duotone fa-regular fa-toolbox text-5xl"></i>
                        <h3 class="text-2xl">Repairs</h3>
                    </div>
                </a>
                <a href="/services">
                    <div class="flex flex-col items-center space-y-2">
                        <i class="fa-sharp-duotone fa-regular fa-repeat text-5xl"></i>
                        <h3 class="text-2xl">Service Plans</h3>
                    </div>
                </a>
            </div>
            <div class="flex flex-row justify-center lg:justify-start space-x-20">
                <button class="px-4 py-4 w-fit bg-amber-300 text-2xl" onclick={() => goto('/contact')}>Book Your Free Quotation!</button>
                <a href="/#company-info"><img class="size-16 object-fill" src={GasSafe} alt=""></a>
            </div>

        </div>
        <div class="h-160 hidden lg:block">
            <img class="object-cover w-full h-full" src={HeroImage} alt="">
        </div>
    </div>
</section>