<script lang="ts">
import { Application, Circle, Sprite, Texture } from 'pixi.js'
import { onMount } from 'svelte';
let canvas: HTMLCanvasElement;

onMount(() => {
    const app = new Application({
      width: 800,
      height: 600,
      backgroundColor: 0x1099bb,
      view: canvas,
    })

    const stage = app.stage;

    const rect = Sprite.from(Texture.WHITE);
    rect.tint = 0xdddddd;
    rect.width = 200;
    rect.height = 200;
    // rect.eventMode = "auto";
    stage.addChild(rect);
    rect.addEventListener("pointerdown", (event) => {
        console.log("moved")
        rect.tint = 0xffffff;
    })
    
    app.ticker.add((dtMs) => {
    })
})

</script>

<canvas class="p-4" bind:this={canvas}/>