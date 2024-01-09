<script>
	export let number;

	$: formattedNumber = number.toLocaleString('de-DE', {
		notation: 'standard',
		compactDisplay: 'short'
	});
</script>

<span>{formattedNumber}</span>

<style>
	span {
		font-variant-numeric: tabular-nums;
	}
</style>
