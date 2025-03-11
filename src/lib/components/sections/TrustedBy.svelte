<script lang="ts">
	import checkatrade from "$assets/checkatrade.webp";
    import ovo from "$assets/ovo.png";
    import refcom from "$assets/refcom.png";
    import glowgreen from "$assets/gg.png";
    import hometree from "$assets/ht.png";
    import verysmart from "$assets/tvshc.png";
    import boxt from "$assets/boxt.png";
    import yourrepair from "$assets/yr.png";
	import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto flex flex-col p-6 xl:flex-row">
		<div class="mb-15 w-full flex items-center space-y-10 text-center xl:mb-0 xl:w-1/2 xl:text-left">
			<Header>Trusted by some of the biggest names in the business!</Header>
		</div>
        <div class="w-full items-center justify-center xl:w-1/2 lg:pl-25">
			<div class="grid grid-cols-3 grid-rows-3 gap-10">
                <div class="size-40">
                    <img src={checkatrade} alt="">
                </div>
                <div class="size-40">
                    <img src={ovo} alt="">
                </div>
                <div class="size-40">
                    <img src={refcom} alt="">
                </div>
                <div class="size-40">
                    <img src={glowgreen} alt="">
                </div>
                <div class="size-40">
                    <img src={hometree} alt="">
                </div>
                <div class="size-40">
                    <img src={verysmart} alt="">
                </div>
                <div class="size-40">
                    <img src={boxt} alt="">
                </div>

                <div class="subgrid col-span-2">
                    <div class="w-85">
                        <img src={yourrepair} alt="">
                    </div>
                </div>
            </div>
		</div>
	</div>
</section>