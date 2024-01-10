<script>
	export let number = 0;

	$: formattedNumber = number
		? number.toLocaleString('de-DE', {
				notation: 'standard',
				compactDisplay: 'short'
			})
		: 0;
</script>

<span>{formattedNumber}</span>

<style>
	span {
		font-variant-numeric: tabular-nums;
	}
</style>
