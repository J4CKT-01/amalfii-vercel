<script lang="ts">
    import HeroImage from '$assets/si-2.jpg';
</script>


<section>
    <div class="container flex flex-col lg:flex-row mx-auto items-center p-6 mt-15">
        <div class="w-full lg:w-1/2 space-y-20 text-center lg:text-left">
        <h1 class="text-9xl font-bold">Amal<span class="text-amber-300">fii</span> Heating</h1>
        <h2 class="text-4xl">Experts in home heating solutions</h2>
        <div class="flex flex-row lg:flex-row space-y-15 justify-evenly lg:justify-start">
            <div class="flex flex-col items-center space-y-2">
                <i class="fa-sharp-duotone fa-regular fa-sign-posts-wrench text-5xl"></i>
                <h3 class="text-2xl">Installations</h3>
            </div>
            <div class="flex flex-col items-center space-y-2 mx-15">
                <i class="fa-sharp-duotone fa-regular fa-toolbox text-5xl"></i>
                <h3 class="text-2xl">Repairs</h3>
            </div>
            <div class="flex flex-col items-center space-y-2">
                <i class="fa-sharp-duotone fa-regular fa-repeat text-5xl"></i>
                <h3 class="text-2xl">Service Plans</h3>
            </div>
        </div>
        </div>
        <div class="w-full lg:w-1/2 flex items-center justify-center">
            <div><img class="object-cover object-right max-h-140 w-full rounded-2xl mb-15" src={HeroImage} alt=""></div>
        </div>
    </div>
</section>