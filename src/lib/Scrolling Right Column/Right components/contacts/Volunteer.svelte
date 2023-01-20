<script>
	import info from "../../../site_info.json";
</script>

<div>
	<h2>Volunteers</h2>
	<div>
		<p>If you would like to volunteer, then please contact us via <a href={info.externalLinkHttps.volunteerSouthLink} target="_blank">Volunteer South</a></p>
		<p>or you can email us directly at 
			<a href={info.plusBusDetails.emailLink}>
				<em>{info.plusBusDetails.email}</em>
			</a>.
		</p>
		<div>
			<h3>We are currently looking for</h3>

			<ul>
				<li>
					<a href={info.assetAdresses.vanDriverPdf} target="_blank">Volunteer Van Driver</a>
				</li>
				
				<li>
					<a href={info.assetAdresses.shoppingAssistantPdf} target="_blank">Volunteer Shopping Assistant</a>
				</li>

				<li>Board Member</li>

				<li>
					<a href={info.externalLinkHttps.volunteerSouthLink} target="_blank">
						<img class="logoVS" src={info.assetAdresses.volunteerSouthLogo} alt="logo">
					</a>
				</li>
			</ul>
		</div>
	</div>
</div>

<style>
	.logoVS {
		width: 200px;
	}
</style>