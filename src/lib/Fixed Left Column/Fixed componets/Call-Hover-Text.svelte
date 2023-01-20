<script>
	import info from "../../site_info.json";
</script>

<div class="callHoverText">
	<p>{info.displayPhoneNumber}</p>
	<p>Office hours are</p>
	<p>
		<strong>{info.openHours[0]}</strong> - <strong>{info.openHours[1]}</strong>
	</p>
</div>

<style>
	.callHoverText {
		text-align: center;
	}
</style>