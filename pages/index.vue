<script setup>
const images = ref([
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123689547126034553/yoguy108_pulse_art_Pantone_color_grades_34041a25-0983-4c97-baba-1a18c88fb8c3.png",
        prompt: "pulse art Pantone color grades:: close-up shot, weird portrait of an ugly idealization::2 unappealing, dark --ar 16:9 --s 800 --q 5 --no woman",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123703763463573555/backtik_Conte_crayon_art_impulse_The_Silent_Celestial_Scribe_No_0d5210c1-e19a-4904-adf7-1c2ee71bf46e.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123711057970614352/rieko.ai_filmstill_photography_impulse_striped_light_stripes_st_e38f3bd4-6ac2-4492-9140-c8dce25f0ff8.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123689547126034553/yoguy108_pulse_art_Pantone_color_grades_34041a25-0983-4c97-baba-1a18c88fb8c3.png",
        prompt: "pulse art Pantone color grades:: close-up shot, weird portrait of an ugly idealization::2 unappealing, dark --ar 16:9 --s 800 --q 5 --no woman",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123703763463573555/backtik_Conte_crayon_art_impulse_The_Silent_Celestial_Scribe_No_0d5210c1-e19a-4904-adf7-1c2ee71bf46e.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123711057970614352/rieko.ai_filmstill_photography_impulse_striped_light_stripes_st_e38f3bd4-6ac2-4492-9140-c8dce25f0ff8.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123703796279803924/backtik_Conte_crayon_art_impulse_The_Silent_Celestial_Scribe_No_68f8b63f-ed10-4714-8c6e-93f8c09637bd.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123711122256703518/rieko.ai_filmstill_photography_impulse_striped_light_stripes_st_9f5662fe-22cf-4921-99b6-10b1d368feb7.png",
        prompt: "rieko.ai filmstill photography impulse stripes stripes",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123703796279803924/backtik_Conte_crayon_art_impulse_The_Silent_Celestial_Scribe_No_68f8b63f-ed10-4714-8c6e-93f8c09637bd.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123711057970614352/rieko.ai_filmstill_photography_impulse_striped_light_stripes_st_e38f3bd4-6ac2-4492-9140-c8dce25f0ff8.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123703796279803924/backtik_Conte_crayon_art_impulse_The_Silent_Celestial_Scribe_No_68f8b63f-ed10-4714-8c6e-93f8c09637bd.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123711122256703518/rieko.ai_filmstill_photography_impulse_striped_light_stripes_st_9f5662fe-22cf-4921-99b6-10b1d368feb7.png",
        prompt: "rieko.ai filmstill photography impulse stripes stripes",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123703796279803924/backtik_Conte_crayon_art_impulse_The_Silent_Celestial_Scribe_No_68f8b63f-ed10-4714-8c6e-93f8c09637bd.png",
        prompt: "Conte crayon art impulse The Silent Celestial Scribe: Noah Bradley Side view Glare and transmitted light Color filters Separation Scheme 4k --ar 16:9 --c 0 --s 750",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123711122256703518/rieko.ai_filmstill_photography_impulse_striped_light_stripes_st_9f5662fe-22cf-4921-99b6-10b1d368feb7.png",
        prompt: "rieko.ai filmstill photography impulse stripes stripes",
    },
    {
        url: "https://cdn.discordapp.com/attachments/945077390839787570/1123496091946598440/pulse_on_the_cover_of_Vogue_fashion_magazine__elegant_hyper_d88df641-82de-4269-a34e-2d6881b40770.png",
        prompt: "pulse on the cover of Vogue fashion magazine: elegant hyper",
    },
]);

const imagesInColumns = computed(() => {
    let copiedImages = [...images.value];
    copiedImages.sort(() => Math.random() - 0.5);

    let columns = [[], [], []];
    copiedImages.forEach((img, index) => {
        columns[index % 3].push(img);
    });

    return columns;
});

function addImage() {
    
}
</script>

<template>
    <div class="header">
        <h1>OMG Midjourey</h1>
        <button @click="addImage">Add image</button>
    </div>

    <div class="image-gallery">
        <div class="column" v-for="(column, i) in imagesInColumns" :key="i">
            <img v-for="(image, j) in column" :src="image.url" :alt="'Image ' + j" :key="j" />
        </div>
    </div>
</template>

<style>
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

h1 {
    font-size: 40px;
    font-family: "Agdasima", sans-serif;
}

.image-gallery {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    gap: 10px;
}

.image-gallery div {
    display: flex;
    flex-direction: column;
    width: 33%;
}

.image-gallery div img {
    width: 100%;
    padding-bottom: 10px;
    transition: filter 0.3s ease-in-out;
}
.image-gallery div img:hover {
    filter: brightness(50%);
}
@media screen and (max-width: 1180px) {
    .image-gallery {
        flex-direction: column;

        gap: 0px;
    }
    .image-gallery div {
        width: 100%;
    }
}
</style>
