<script>
export let data;
export let xScale;
export let yScale;
</script>

<div class='tooltip' 
		 style="position: absolute;
						top: {yScale(data.hours)}px;
						left: {xScale(data.grade)}px;">
<p><strong>{data.name}</strong></p> 
<p>{data.hours} hours studied</p>
</div>

<style>
	.tooltip {
		padding: 6px;
		background: white;
		border: 1px solid rgba(0,0,0,0.5);
		pointer-events: none;
		transition: top 300ms ease, left 300ms ease;
	}
	p {
		margin: 0px;
	}
</style>