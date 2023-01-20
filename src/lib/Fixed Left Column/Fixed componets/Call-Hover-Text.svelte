<script>
	export let openHours;
	export let displayPhoneNumber;
</script>

<div class="callHoverText">
	<p>{displayPhoneNumber}</p>
	<p>Office hours are</p>
	<p>
		<strong>{openHours[0]}</strong> - <strong>{openHours[1]}</strong>
	</p>
</div>

<style>
	.callHoverText {
		text-align: center;
	}
</style>