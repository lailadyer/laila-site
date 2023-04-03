<script lang="ts">
    const loremIpsum = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.";
    let loremIpsumArray: string[] = [];
    for (let index = 0; index < 40; index++) {
        loremIpsumArray.push(loremIpsum);
    }
</script>

<div class="bg-pink-300">
    <h2 class="m-3 text-center">Laila's corner of the internet</h2>
</div>
{#each loremIpsumArray as p}
    <p class="mt-0 mb-4 opacity-0">{p}</p>
{/each}

<style lang="postcss">
    :global(body) {
        font-family: Capriola;
        margin: 0;
        background-image: url("./images/background/pink clouds.jpg");
        background-size: cover;
        backdrop-filter: blur(2em);
    }
</style>