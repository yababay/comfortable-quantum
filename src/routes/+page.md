---
title: Комфортабельные кванты
description: Лента времени, иллюстрирующая развитие квантовой физики от «булки с изюмом» до нобелевской премии 2022 г.
---

<script>
    import { onMount } from 'svelte'
    import Helper from '$lib/components/Helper.svelte' 
    import draw from './draw.js'
    import './timeline.css'

    export let data

    const { title, description, banner, image } = data

    onMount(() => {
        draw(div)
    })

    let div 

</script>

<Helper {title} {description} {banner} {image} />

<div id="timeline" bind:this={div}></div>
