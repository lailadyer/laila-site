<script lang="ts">
	import PixiJs from "$lib/PixiJs.svelte";

    
</script>
<div class="bg-gradient-to-br from-pink-100 to-pink-300 min-h-screen m-0 p-0">
    <div class="p-4">
        <h2 class="bg-pink-200 p-4 text-center text-2xl border-8 border-white rounded-lg">Laila's corner of the internet</h2>
    </div>
    <div class="flex flex-row justify-center">
        <div class="m-8 border-8 border-white bg-pink-200 shadow-md rounded-xl">
            <p class="p-8">Let's try out some PixiJs on the right here -></p>
        </div>
        <div class="m-8 border-8 border-white bg-pink-200 shadow-md rounded-xl flex-grow">
            <PixiJs />
        </div>
    </div>
</div>

<style>
    :global(body) {
        font-family: Capriola;
        margin: 0;
    }
</style>