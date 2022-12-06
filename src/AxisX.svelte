<script>
let xTicks = [0, 25, 50, 75, 100];
export let height;
export let xScale;
export let margin;
</script>



<g>
	{#each xTicks as tick}
		<text x={xScale(tick)} 
					y={height - margin.bottom}
					dy="6"
					dominant-baseline="hanging"
					>{tick}%</text>
	{/each}
</g>