<script>
    import Gallerycard from "$lib/components/gallerycard.svelte";
    let poster;
    //import "$lib/assets/hactus_poster.webp";
    //
    import { scale } from "svelte/transition";
    import { quintOut } from "svelte/easing";
    import { Gallery } from "flowbite-svelte";

    let index = $state(0);
    import {
        Carousel,
        Controls,
        Thumbnails,
        CarouselIndicators,
    } from "flowbite-svelte";
    const images = [
        {
            alt: "Intro",
            src: "/src/lib/assets/The_hactus_poster_small.webp",
            title: "intro",
        },
        {
            alt: "asterisk",
            src: "/src/lib/assets/asterisk_small.webp",
            title: "asterisk",
        },
        {
            alt: "coral",
            src: "/src/lib/assets/coral.png",
            title: "coral",
        },
    ];
    //import images from "./images.json";
</script>

<main>
    {#if true}
        <header>
            <h1>Hactus Design</h1>
        </header>
        <main>
            <Gallery items={images} />
            <!-- --
            <Carousel {images} transition={scaleAnimation}>
                <div class="d">
                    <Controls />
                </div>
            </Carousel>

             --
                    <div class="gallery-box">
                        <h1>Intro</h1>
                        <img
                            src="/src/lib/assets/The_hactus_poster.webp"
                            alt=""
                            class="image"
                        />
                    </div>
                    <div class="gallery-box">
                        <h1>3*S</h1>
                        <img
                            src="/src/lib/assets/asterisk.webp"
                            alt=""
                            class="image"
                        />
                    </div>-->
        </main>
        <footer></footer>
    {/if}

    <!-- --
    <h1>header</h1>
    <h2>header</h2>
    <h3>header</h3>
    <h4>header</h4>
    <h5>header</h5>
    <h6>header</h6>
    <p>paragraph</p>
    <button on:click={scrollTo(0, 50)}>scroll</button>
    -->
</main>

<style>
    .image {
        width: 75%;
    }
    main {
        width: 100rem;
    }
    .d {
        width: 100vw;
        display: flex;
    }
</style>
