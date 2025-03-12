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
	<div class="container mt-5 lg:mt-15 mx-auto flex flex-col p-2 lg:p-6 lg:flex-row">
		<div class="my-20 w-full flex items-center space-y-10 text-center xl:my-0 lg:w-1/2 xl:text-left">
			<Header>Trusted by some of the biggest names in the business!</Header>
		</div>
        <div class="w-full items-center justify-center lg:w-1/2 border rounded-3xl overflow-hidden p-10">
			<div class="grid">
                <div>
                    <img class="object-fill" src={ovo} alt="">
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
                        <img class="w-full" src={yourrepair} alt="">
                </div>
            </div>
		</div>
	</div>
</section>