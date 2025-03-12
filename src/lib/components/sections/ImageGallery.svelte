<script lang="ts">
    import office2 from '$assets/gallery/office-2.jpg';
    import office4 from '$assets/gallery/office-4.jpg';
    import si1 from '$assets/gallery/si-1.jpg';
    import visit1 from '$assets/gallery/visit-1.jpg';
    import visit2 from '$assets/gallery/visit-2.jpg';
    import { Header } from '$lib';
</script>

<section>
	<div class="container mx-auto mt-5 lg:mt-15 p-2 lg:p-6 mb-5 lg:mb-15">
        <div class="w-full text-center mb-15"><Header>See our team in action!</Header></div>
        <div class="grid grid-cols-2 lg:grid-cols-4 gap-10">
            <div>
                <img class="h-100 min-w-full object-cover rounded-3xl" src={office2} alt="">
            </div>
            <div>
                <img class="h-100 min-w-full object-cover rounded-3xl" src={office4} alt="">
            </div>
            <div>
                <img class="h-100 min-w-full object-cover rounded-3xl" src={si1} alt="">
            </div>
            <div>
                <img class="h-100 min-w-full object-cover rounded-3xl" src={visit1} alt="">
            </div>
        </div>
    </div>
</section>