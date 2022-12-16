<script lang="ts">
    export let src: string;
    export let alt: string;
</script>

<img src={src} alt={alt} />

<style>
    img {
        max-width: 100%;
        width: 100%;
        height: 100%;
        max-height: 100%;
        object-fit: contain;
    }
</style>