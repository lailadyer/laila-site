<script lang="ts">
    import noteBackground from "$lib/images/backgrounds/note-background.png"

    const loremIpsum = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.";
    let loremIpsumArray: string[] = [];
    for (let index = 0; index < 40; index++) {
        loremIpsumArray.push(loremIpsum);
    }
</script>

<div class="bg-pink-300 m-8 text-2xl font-bold">
    <h2 class="p-4 text-center ">Laila's corner of the internet</h2>
</div>
{#each loremIpsumArray as p}
<div class="m-8 bg-repeat bg-contain shadow" style="background-image: url({noteBackground})">
    <p class="p-8 opacity-100">{p}</p>
</div>
{/each}

<style>
    :global(body) {
        font-family: Capriola;
        margin: 0;
        background-image: url($lib/images/backgrounds/page-background.jpg);
        background-size: cover;
        backdrop-filter: blur(2rem);
    }
</style>