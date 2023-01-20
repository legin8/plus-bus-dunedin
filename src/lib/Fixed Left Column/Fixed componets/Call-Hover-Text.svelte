<script>
	import info from "../../site_info.json";
</script>

<div class="callHoverText">
	<p>{info.displayPhoneNumber}</p>
	<p>Office hours are</p>
	<p>{info.officeHourDaysMessage}</p>
	<p>
		<strong>{info.officeHourTimesMessage}</strong>
	</p>
</div>

<style>
	.callHoverText {
		text-align: center;
	}
</style>