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
			<div class="grid grid-cols-2 grid-rows-3 lg:grid-cols-3 lg:grid-rows-3 gap-10">
                <div>
                    <img src={ovo} alt="">
                </div>
                <div>
                    <img src={refcom} alt="">
                </div>
                <div>
                    <img src={glowgreen} alt="">
                </div>
                <div>
                    <img src={hometree} alt="">
                </div>
                <div>
                    <img src={verysmart} alt="">
                </div>
                <div>
                    <img src={boxt} alt="">
                </div>

                <div class="subgrid col-span-3">
                        <img src={yourrepair} alt="">
                </div>
            </div>
		</div>
	</div>
</section>