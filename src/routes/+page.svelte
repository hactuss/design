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
    /*
    const images = [
        {
            alt: "Intro",
            src: "/src/lib/assets/hactus_poster.webp",
            title: "intro",
        },
        {
            alt: "asterisk",
            src: "/src/lib/assets/asterisk.webp",
            title: "asterisk",
        },
        {
            alt: "coral",
            src: "/src/lib/assets/coral.png",
            title: "coral",
        },
        {
            alt: "obnitem",
            src: "/src/lib/assets/Obnite.webp",
            title: "obnitem",
        },
        {
            alt: "secretcode",
            src: "/src/lib/assets/secretcodeofhactuss.png",
            title: "secretcode",
        },
        ];*/
    //import images from "./images.json";
</script>

<main>
    {#if true}
        <header>
            <h1>Hactus Design</h1>
        </header>
        <main>
            <div class="gallery">
                <img src="../lib/assets/hactus_poster.webp" alt="intro" />
                <br />
                <img src="../lib/assets/asterisk.webp" alt="asterisk" />
                <br />
                <img src="../lib/assets/Obnite.webp" alt="obnitem" />
                <br />
                <img src="../lib/assets/coral.png" alt="coral" />
                <br />
                <img src="../lib/assets/secretcodeofhactuss.png" alt="code" />
            </div>
            <!--
            <Gallery items={images} />

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
    img {
        width: 100%;
    }
    main {
        width: 100rem;
    }
    .gallery {
        display: flex;
        flex-direction: column;
        width: 50vw;
    }
</style>
