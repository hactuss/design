<script>
    let image_url = $props();
    console.log(image_url);
</script>

<main>
    <img src={image_url} alt={image_url} />
</main>

<style>
    main {
        background: url({image_url});
    }
</style>
